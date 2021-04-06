dlevikov Infra repository

bastion_IP = 130.193.49.68
someinternalhost_IP = 10.130.0.25
testapp_IP = 178.154.201.239
testapp_port = 9292

connect to someinternalhost into one command:
ssh -i ~/.ssh/appuser -A appuser@130.193.49.68 -t ssh appuser@10.130.0.25


с помощью образа из предыдущего домашнего задания и терраформа, подняли виртуальную машину.
В качестве самостоятельной работы настроили переменные
