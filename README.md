dlevikov Infra repository

bastion_IP = 130.193.49.68
someinternalhost_IP = 10.130.0.25

connect to someinternalhost into one command:
ssh -i ~/.ssh/appuser -A appuser@130.193.49.68 -t ssh appuser@10.130.0.25
