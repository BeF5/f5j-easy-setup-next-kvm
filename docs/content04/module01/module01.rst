BIG-IP Next VE KVMのインストール
=========================================================

KVMサポートに関する情報をご説明します。

詳細に関しては、原文 `Official Docs`_  をご参照ください。

.. list-table:: KVMシステム要件と互換性
   :widths: 25 50
   :header-rows: 1

   * - 項目
     - 説明
   * - ハイパーバイザー
     - KVM QEMU 6.2 on Ubuntu 22.04
   * - サーバチップセット
     - i440fx または q35
   * - CPU
     - 2 vCPUs以上
   * - メモリ
     - 8GB以上
   * - ディスク容量
     - 80GB以上
   * - HA構成
     - ノード３台
   * - ネットワーク・インタフェース
     -  2つ以上
   * - ネットワーク・ドライバ
     - virtio (SR-IOVは未サポート)
 

.. list-table:: テナントのサイズに関して
   :widths: 25 25
   :header-rows: 1

   * - vCPUs
     - Memory
   * - 2
     - 8GB
   * - 4
     - 10GB
   * - 6
     - 12GB
   * - 8
     - 16GB
   * - 12
     - 24GB
   * - 16
     - 32GB
   * - 24
     - 48GB



.. _Official Docs: https://clouddocs.f5.com/bigip-next/latest/install/big_ip_next_supported_platforms.html
 


