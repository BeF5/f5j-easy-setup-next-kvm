BIG-IP Next VE KVMのインスタンスのLicenseに関して
================================================

本章では、BIG-IP Next VEのライセンスのアクティベーションをします。


F5 アイコンの隣にあるワークスペース アイコンをクリックし、Infrastructure >> Instances >> My Instances画面を表示します。

.. image:: images/Picture1.png
  :scale: 90%
  :align: center

.. image:: images/Picture2.png
  :scale: 90%
  :align: center
|       


前に追加したインスタンスの名前をクリックします。


.. image:: images/Picture3.png
  :scale: 90%
  :align: center
|       


次に、Licenseをクリックします。ステータスが「非アクティブ」になっていることがわかります。

.. image:: images/Picture4.png
  :scale: 90%
  :align: center
|       

Active Licenseをクリックすると、ライセンス要件の概要が表示されます (ライセンスのアクティブ化ワークフローを初めて実行する場合)。

.. image:: images/Picture5.png
  :scale: 90%
  :align: center
|       


NextをクリックしてNew Token(JWT)を選択して、トークンの欄にペーストします。

.. image:: images/Picture6.png
  :scale: 90%
  :align: center
|       

kvm-testという名前を入力します。

Activateをクリックします。

Activate完了後にStatusがActiveと表示されます。

.. image:: images/Picture7.png
  :scale: 90%
  :align: center
|       