
## CREATING INFRASTRCTURE IN AWS

### STEP 1: Create a terraform repository
* added gitignore
<img width="951" alt="one terraform repo" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/3f5e0706-0a08-494c-bcf0-01ae40cbdf27">

* Open codespace sandbox
<img width="938" alt="two set up code space" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/d623c6e5-d86b-4930-999b-4a047ef3546b">

* Connected on codespace sanbox
<img width="926" alt="three codespace opened" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/64392a64-d523-4dea-af65-7e77cdf3752e">

### STEP 2 : Install terraform
* type "> dev" on the top bar
* click on first option, codespaces: Add Dev Container Configuration Files
* click on modify your active configuration
* After clicking on the terraform official application with the checkmark
* click ok
* Next click keep default
<img width="952" alt="four install terra form" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/f9b1c1dd-7ed8-4728-b229-ccaec2485f89">

* Terraform is installed
<img width="955" alt="five it created  a devcontainerfile dot json" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/28f8742c-d9f2-476d-87db-1e7a3c9a72d3">

### STEP 3: AWS CLI Installation

### Since I Want To Create Infrastruction In AWS, Terraform Needs To Communicate With AWS, Hence The Installation Of AWS CLI

* Following same process of installing terraform to install AWS CLI 
<img width="916" alt="six install AWS CLI" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/572e2b45-9010-42f7-ba13-dbe5b14f70d0">

* Aws Cli installed
<img width="926" alt="seven AWS CLI installed" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/c3faa922-bc20-40b5-9f5e-57cf5c8fa220">

* Refresh to Rebuild container
 <img width="958" alt="eight click to rebuild container" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/623b2be7-4236-4496-a91e-0aeeb6e7a330">

* Rebuiulding is  processing
<img width="941" alt="Nine container rebuilding" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/b3910341-de0c-4577-89eb-20976498d020">

* Checking terraform and AWS CLI version
<img width="869" alt="ten terraform and aws cli installed" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/dc8fc343-ecf3-4d95-b52d-c85a8c08be48">

### STEP 4: CREATE AN IAM USER

* Create an user
<img width="928" alt="11 choose an existing  user or create a new user" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/5d791eff-2f77-47ae-89a6-0ecfd113a471">

 *  Give it a name "my-terraform-user"
<img width="919" alt="12 create IAM user" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/daa359c4-f1be-488a-aea6-a9ec2cede0f6">

* Set permissions
* Attach direct policies
<img width="943" alt="13 attach policies directly" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/b97dc448-de8c-4bc6-88e6-dc2f0ea23a8d">

* Grant user ec2 full access policy
<img width="601" alt="aws config b" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/ef38a2b2-b863-4df7-87b9-84a976f13093">

* Grant user S3 full access permissiom
<img width="926" alt="14b and s3 full access permision" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/428d8b31-9be0-4c0f-90d3-d883e3144558">

* Review and create permission policies 
<img width="920" alt="14c review permission policies and create" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/22ed0118-9739-455d-a497-6df86564170d">

* My-terraform-user created
<img width="948" alt="14d user succeefully created" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/f3c2186e-45e1-442c-9632-0dc02557ea2c">


*  View my-terraform-user summary
*  Create access key
<img width="938" alt="14ee create access key" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/b68d3870-a82b-40f1-a6aa-35eadc08b96a">

* Click security credentials
* Click on command line interface cli
<img width="959" alt="15 click on cli tick confirm and create" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/8d72c8b1-44ca-4e8a-b5dc-72e592f07209">

* Create descriptive tag "tarraform-creation"
* Create access key
<img width="945" alt="16 give it a tag" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/4c0ec3a8-6939-431d-97e9-bd132657941d">

* Access created
<img width="924" alt="17 key created and downloaded" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/0d1c9684-8911-4bdf-8b18-83fbc455cdf7">

* Access key downloaded
* Click down
<img width="952" alt="17b" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/6e33e472-c774-4314-8141-522c3e829669">

 ### STEP 5 : On a broswer, Type Terraform Provider and go to AWS Documentation
 * Copy the IAM user code resource
<img width="936" alt="18 copy iam user code from terraform aws" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/aba56c5e-531c-4eec-9385-da634bada677">

* On a broswer, type terraform provider, go to AWS documentation, locate AWS tarraform provider configuration code
<img width="951" alt="terraform provider installation configuration" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/c4814be2-78b7-43c4-a72d-48bd75b4fae4">

* Head over to code your repository, go to codespace,
* On terraform-project, create a file called "main.tf" 
<img width="958" alt="18 created afolder and a file inside the folder" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/a01e9f14-8e22-4974-89d6-f75c951fc2c1">


* Paste both the Terraform provider configuration code and the AWS provider configuration code
* This is not actually the best practice to, expose my access and security keys. 
<img width="956" alt="18 its not actually best pratice to past both keys there so i opt for another way" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/d4334341-5ab6-4eb9-a0ae-eced807e778f">

* This is a better practice, by using profile instead of access and seccurity keys
<img width="832" alt="18b change keys to profile for security reasons" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/b39d46d4-96a7-475a-b692-d09a68a764b4">

* ls to view terraform=project folder
<img width="951" alt="19" src="https://github.com/Gailpositive/terraform-deployment/assets/111061512/b6160382-0f5b-4d04-b807-516cdf2c256d">
