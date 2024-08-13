BIG-IP Next VE KVMのイメージ作成
=========================================================

ダウンロードされたイメージを解凍します。


例:

    .. code-block:: bash

        tar -xvf BIG-IP-Next-20.2.1-2.430.2+0.0.48.qcow2.tar.gz

 
.. image:: images/Picture1.png
   :scale: 20%
   :align: center
|

cpコマンドで新規イメージを作成します。

例:

    .. code-block:: bash

        cp BIG-IP-Next-20.2.1-2.430.2+0.0.48.qcow2.tar.gz my-bigip-next.qcow2


.. image:: images/Picture2.png
   :scale: 20%
   :align: center
|

cloud-localdsというツールをインストールして事前に作成したnetplanファイルを指定してISOイメージを作成(cloud-localds は、ユーザーデータやメタデータを含むディスクイメージを作成します)


例:

    .. code-block:: bash

        sudo apt install cloud-image-utils

        cloud-localds my-bigip-next.iso -H my-bigip-next -N network.yaml -m local /dev/null

.. image:: images/Picture3.png
   :scale: 20%
   :align: center
|