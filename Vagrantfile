VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
        config.vm.box = "centos5.8"
        config.vm.network "public_network",
        ip: "172.16.41.137",netmask: "255.255.252.0"

        if Vagrant.has_plugin?("vagrant-proxyconf")
             config.yum_proxy.http = "http://172.16.40.1:8888/"
             config.proxy.http     = "http://172.16.40.1:8888/"
             config.proxy.https    = "http://172.16.40.1:8888/"
             config.proxy.no_proxy = "localhost,127.0.0.1,.it-college.local" 
        end
  end
#vagrant halt     => 停止 
#vagrant init     => 追加
#vagrant destroy  => initしたものを削除
