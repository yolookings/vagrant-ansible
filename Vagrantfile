Vagrant.configure("2") do |config|

  config.vm.define "satu" do |h1|
    h1.vm.hostname = "satu-host"
    h1.vm.box = "aspyatkin/ubuntu-20.04-server"
  end
  
  config.vm.define "dua" do |h2|
    h2.vm.hostname = "dua-host"
    h2.vm.box = "aspyatkin/ubuntu-20.04-server"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yaml"
  end

end
# Lakukanlah provision pada 2 VM dengan OS Ubuntu Focal Fossa menggunakan Ansible Playbook dan KVM + Virtual Machine Manager dengan menginstall Apache2 dan Bind9 (Note: Seluruh provisioning dan konfigurasi untuk semua vm disatukan pada satu Ansible Playbook)
