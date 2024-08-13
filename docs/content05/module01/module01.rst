BIG-IP Next VE KVMのインスタンスのOnboarding
=========================================================

Postmanというツールを使用して、BIG-IP Next VEのAPIに対して設定パラメータを送信してonboardingします。

下記URLにてPostmanのcollectionをダウンロードしてPostmanのアプリにインポートします。
 `BIG-IP Next Postman Collection`_  

.. image:: images/Picture1.png
  :scale: 90%
  :align: center


.. image:: images/Picture2.png
  :scale: 90%
  :align: center
|       

.. image:: images/Picture3.png
  :scale: 90%
  :align: center
|       

Postmanアプリの右上にある環境変数アイコンをクリックして、使用するBIG-IP Next IPアドレスやパスワードの値を変更します。

.. image:: images/Picture4.png
  :scale: 90%
  :align: center
|   


Postman Collectionを開いてonboarding用の項目を確認します。

.. image:: images/Picture5.png
  :scale: 90%
  :align: center
|   

Reset Admin Password, Login, Check Health, Onboarding, Check Onboarding Jobのリクエストを順番に実行します。

.. image:: images/Picture6.png
  :scale: 90%
  :align: center
|   

.. image:: images/Picture7.png
  :scale: 90%
  :align: center
|   

.. image:: images/Picture8.png
  :scale: 90%
  :align: center
|   

.. image:: images/Picture9.png
  :scale: 90%
  :align: center
|   


Check Onboarding JobのリクエストのTest Resultsが全てPASSとなっていることを確認します。


.. image:: images/Picture10.png
  :scale: 90%
  :align: center
|   

.. image:: images/Picture11.png
  :scale: 90%
  :align: center
|   

PostmanによるOnboarding後、BIG-IP Next Central Manager に管理者としてログインし、F5 アイコンの隣にあるワークスペース アイコンをクリックし、Infrastructure >> Instances >> My Instances画面を表示します。

.. image:: images/Picture12.png
  :scale: 90%
  :align: center
|   

Start Adding Instancesをクリックして事前に起動したインスタンスのIPアドレスとポートを入力してConnectを押下します。

.. image:: images/Picture13.png
  :scale: 90%
  :align: center
|   

.. image:: images/Picture14.png
  :scale: 90%
  :align: center
|   

インスタンスのユーザ名とパスワードを入力します。

.. image:: images/Picture15.png
  :scale: 90%
  :align: center
|  

Add Instance画面にて新たに管理用のユーザ名とパスーどを入力
(既存に表示されるadmin-cmのユーザ名を使用することを推奨します。)

.. image:: images/Picture16.png
  :scale: 90%
  :align: center
|  

インスタンスの一元管理を確認するように求められます。 BIG-IP Next Central Manager は、追加している BIG-IP Next インスタンスからローカルに構成されたユーザーをすべて削除します。何らかの理由で、ローカルの BIG-IP Next インスタンスでのユーザーの無効化が失敗した場合、BIG-IP Next インスタンスの BIG-IP Next Central Manager への追加は停止され、ローカルの BIG-IP Next インスタンスですべてのユーザーが再度有効になります。 。この確認ダイアログではAddをクリックする必要があります。

.. image:: images/Picture17.png
  :scale: 90%
  :align: center
|  

Continue Connecting?という画面にてNodeのFingerprintを確認してAcceptを押下します。

.. image:: images/Picture18.png
  :scale: 90%
  :align: center
|  

.. image:: images/Picture19.png
  :scale: 90%
  :align: center
|  

この手順を完了すると、My Instancesのリストに新しいインスタンスが表示されます。

.. image:: images/Picture20.png
  :scale: 90%
  :align: center
|  

.. _BIG-IP Next Postman Collection: https://clouddocs.f5.com/bigip-next/latest/_downloads/97786c6c678c239863323f200a105b6f/BIG-IP-Next-Postman-Collection-v20.2.1-4.15.68-0.0.1.zip

 


