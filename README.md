dlevikov Infra repository

bastion_IP = 130.193.49.68
someinternalhost_IP = 10.130.0.25

connect to someinternalhost into one command:
ssh -i ~/.ssh/appuser -A appuser@130.193.49.68 -t ssh appuser@10.130.0.25

testapp_IP = 178.154.203.104
testapp_port = 9292

Доп. задание:
yc compute instance create \
  --name reddit-app \
  --hostname reddit-app \
  --memory=4 \
  --create-boot-disk image-folder-id=standard-images,image-family=ubuntu-1604-lts,size=10GB \
  --network-interface subnet-name=default-ru-central1-a,nat-ip-version=ipv4 \
  --metadata serial-port-enable=1 \
  --metadata-from-file user-data=./metadata.yml
