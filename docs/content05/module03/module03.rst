BIG-IP Next VE KVMのネットワーク・インターフェース設定
=========================================================

インスタンスのNetworking & Proxyをクリックするとvirt-installコマンドで定義したインターフェースの確認が可能です。

 
.. image:: images/Picture1.png
   :scale: 90%
   :align: center
|


外部(dataplane)通信用のインターフェースの設定を行う。

Edit >> Networking

下記の順で設定を入力

#. L1 Networks
#. VLANs
#. IP Addresses


 
.. image:: images/Picture2.png
   :scale: 90%
   :align: center
|


L1 Networks設定後に、次にVLANs設定に進みます。


.. image:: images/Picture3.png
   :scale: 90%
   :align: center
|

VLAN設定を入力します。


.. image:: images/Picture4.png
   :scale: 90%
   :align: center
|

2つ目のネットワークブリッジに所属しているサブネットのIP Addressを入力し、Nextを押下します。

.. image:: images/Picture5.png
   :scale: 90%
   :align: center
|

最後にDeployを押下します。


.. image:: images/Picture6.png
   :scale: 90%
   :align: center
|