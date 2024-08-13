BIG-IP Next Central Manager KVMのデプロイ
=========================================================


以下のようなコマンドでNext CMのqcow2イメージを指定してインスタンスのデプロイを実施


    .. code-block:: bash

        virt-install --name cm1 --memory 16384 --vcpus 8 --disk BIG-IP-Next-CentralManager-20.2.1-0.3.25.qcow,bus=sata --import --os-variant ubuntu22.04 --network=bridge=ovs-mgmt,model=virtio,virtualport_type=openvswitch --noreboot --noautoconsole


.. list-table:: オプションの説明
   :widths: 25 50
   :header-rows: 1

   * - オプション名
     - 説明
   * - --noautoconsole
     - ゲスト起動時ホストからゲストにコンソール接続するのを抑制
   * - --noreboot
     - インストール後はVMを停止する
   * - --network
     - ゲストからホストへのネットワーク接続を指定
   * - --os-variant 
     - OS細部種類を指定
   * - --import 
     - ボリュームをインポート

