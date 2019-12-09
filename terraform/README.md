export GOOGLE_REGION=us-east1-b
export TF_VAR_org_id=198166
export TF_VAR_billing_account=0185A7-9F44C2-66FA56
export TF_VAR_region=${GOOGLE_REGION}
export TF_VAR_user=${USER}
export TF_VAR_ssh_key=/home/ec2-user/gcp/gcp.rsa.pub
export TF_ADMIN=${USER}-tf-admin
export TF_CREDS=/home/ec2-user/gcp/gcp.json


-generate the key
ssh-keygen -t rsa -b 4096 -f gcp_rsa


wget http://distfiles.macports.org/google-cloud-sdk/google-cloud-sdk-272.0.0-darwin-x86_64.tar.gz

tar zxvf google-cloud-sdk-272.0.0-darwin-x86_64.tar.gz

sudo yum install python36

./google-cloud-sdk/install.sh

cd google-cloud-sdk
./google-cloud-sdk/install.sh
安装脚本很快，可以在Linux系统上彻底设置SDK，完成后，访问它：
gcloud init



Did not print [12] options.
Too many options [62]. Enter "list" at prompt to print choices fully.
Please enter numeric choice or text value (must exactly match list
item):  1

Your project default Compute Engine zone has been set to [us-east1-b].
You can change it by running [gcloud config set compute/zone NAME].

Your project default Compute Engine region has been set to [us-east1].
You can change it by running [gcloud config set compute/region NAME].

Created a default .boto configuration file at [/home/ec2-user/.boto]. See this file and
[https://cloud.google.com/storage/docs/gsutil/commands/config] for more
information about configuring Google Cloud Storage.
Your Google Cloud SDK is configured and ready to use!

* Commands that require authentication will use wang.ming.0483@gmail.com by default
* Commands will reference project `modern-webbing-261406` by default
* Compute Engine commands will use region `us-east1` by default
* Compute Engine commands will use zone `us-east1-b` by default

Run `gcloud help config` to learn how to change individual settings

This gcloud configuration is called [default]. You can create additional configurations if you work with multiple accounts and/or projects.
Run `gcloud topic configurations` to learn more.

Some things to try next:

* Run `gcloud --help` to see the Cloud Platform services you can interact with. And run `gcloud help COMMAND` to get help on any gcloud command.
* Run `gcloud topic --help` to learn about advanced features of the SDK like arg files and output formatting