事前準備
=========================================================

KVMイメージを操作するためのツールを事前にインストールしてください。

- virtinst
- virt-inst
- virt-viewer
- virsh
- cloud-localds
- ovs-vsctl (またはbrctl)


KVMサーバ上に、BIG-IP Next CMインスタンスのイメージをインポートしておきます。

Central Manager用のqcowのイメージは、MyF5からダウンロード可能です。

Resource >> Download

   .. image:: images/Picture1.png
      :scale: 90%
      :align: center


   .. image:: images/Picture2.png
      :scale: 90%
      :align: center
   |       


Copy Download Linkを使用してサーバから直接ダウンロードすると簡単にファイルの取り込みが可能です。


   .. image:: images/Picture3.png
      :scale: 90%
      :align: center
   |       


   .. image:: images/Picture4.png
      :scale: 90%
      :align: center
   |       


サーバ上に、ネットワークBridgeを作成しておきます。

- CMとVEの管理インターフェース用
- brctl もしくはovs-vsctlコマンドでbridge作成は可能

例: 

    .. code-block:: bash

        sudo ovs-vsctl add-br ovs-mgmt

        sudo ovs-vsctl add-port ovs-mgmt eno1





