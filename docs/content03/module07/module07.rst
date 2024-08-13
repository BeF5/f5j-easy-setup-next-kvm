BIG-IP Next Central Manager KVMのGUIでのセットアップ
=========================================================

CMの様々なサービスをインストールするためにSet Upボタンを押下します。

.. note::

   注記: 事前にCLIで行われたsetupスクリプトが完了後に２−３分待ってからこちらのGUIでのSet Upを実施してください。




.. image:: images/Picture1.png
   :scale: 80%
   :align: center
|



セットアップに必要な情報を確認後にNextを押して続けます。


.. image:: images/Picture2.png
   :scale: 80%
   :align: center
|


Standalone構成の場合は1台のCMサーバの状態がReadyであることを確認します。

任意: 外部Storage(NFSまたはSAMBA)を設定したい場合はStorageを選択して設定を行います。

Start CM Servicesを押してセットアップを実施


.. image:: images/Picture3.png
   :scale: 80%
   :align: center
|

High Availability構成の場合は+AddボタンをクリックしてCMノードを追加します。

.. image:: images/Picture4.png
   :scale: 80%
   :align: center
|

Continue Connecting?という画面にてNodeのFingerprintを確認してAcceptを押下します。

.. note::

   注記: ノードの追加には所要時間は15分程度

.. image:: images/Picture5.png
   :scale: 80%
   :align: center
|


セットアップ実行中にはこのような画面にて状態の確認が可能です。

.. image:: images/Picture6.png
   :scale: 80%
   :align: center
|

CMのCLIにてkubectlコマンドでpodの起動状態の確認も可能です。

.. image:: images/Picture7.png
   :scale: 80%
   :align: center
|

セットアップ実行中にはこのような画面にて状態の確認が可能です。

.. image:: images/Picture8.png
   :scale: 80%
   :align: center
|

インストール後、BIG-IP Next Central Manager に管理者としてログインし、F5 アイコンの隣にあるワークスペース アイコンをクリックし、

.. image:: images/Picture9.png
   :scale: 80%
   :align: center
|

システム >> CM Maintenanceをクリックして、Setup画面をクリックすると、Bootstrap Statusが完了と表示されます。

.. image:: images/Picture10.png
   :scale: 80%
   :align: center
|

