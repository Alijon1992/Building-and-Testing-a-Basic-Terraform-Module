# Building-and-Testing-a-Basic-Terraform-Module

In this hand-on section will will follow the following steps:

1) Build terraform main project directory.

2) Within this directory will create a subdirectory which will house all our modules.

3) Inside this subfolder will create "main.tf", "variables.tf", and "outputs.tf" files.

4) Then we will paste the given codes inside the created files properly.

5) Finally, we will check AWS console for our created resources.

LET`S GET STARTED!!!

--First make sure you have installed terraform. To do that write command "terraform version"

<img width="400" alt="Screenshot 2023-03-13 at 7 54 50 PM" src="https://user-images.githubusercontent.com/121365233/224857488-74c1c260-1c1d-4a4f-a4d0-c7875347d9f1.png">

--create main(housing) directory.

<img width="369" alt="Screenshot 2023-03-13 at 9 38 22 PM" src="https://user-images.githubusercontent.com/121365233/224869930-8159e470-98d2-49d3-bd39-d16f8f7459a3.png">

--Now, let’s get dive into the "terraform_project" directory

<img width="361" alt="Screenshot 2023-03-13 at 9 39 23 PM" src="https://user-images.githubusercontent.com/121365233/224870056-3572d39c-0f1a-4b39-97e6-152ed442b9f8.png">

--Within this directory let’s created subdirectory which hosts our codes. (Actually here we are creating one more folder inside "modules"folder just in case of created more than one modules and keeping them in the same folder.)

<img width="475" alt="Screenshot 2023-03-13 at 9 45 33 PM" src="https://user-images.githubusercontent.com/121365233/224870860-e4b19bc7-85ac-4687-824c-cf41ba7f3f69.png">

--Time to change directory into "vpc"

<img width="592" alt="Screenshot 2023-03-13 at 9 48 38 PM" src="https://user-images.githubusercontent.com/121365233/224871301-88cd7072-9d34-4f5a-9fcb-8c9ce3e03651.png">

--Create "main.tf" file and paste the code that I have provided for you in "additional resources". Then save and exit! To do that press esc-->:wq

<img width="294" alt="Screenshot 2023-03-13 at 9 54 26 PM" src="https://user-images.githubusercontent.com/121365233/224872088-82fd5f39-e656-46ce-80a4-99c4076b44b5.png">

<img width="614" alt="Screenshot 2023-03-13 at 9 55 12 PM" src="https://user-images.githubusercontent.com/121365233/224872232-59a1f41a-adaa-428f-9465-ee221a5bc4a9.png">

--Create "variables.tf" file and paste related codes from "Additional resources" doc. that I have provided for you. Then save and quit.

<img width="333" alt="Screenshot 2023-03-13 at 10 13 40 PM" src="https://user-images.githubusercontent.com/121365233/224875133-e60a7db5-46ff-4d49-9964-dac37c2f5e85.png">

<img width="217" alt="Screenshot 2023-03-13 at 10 14 45 PM" src="https://user-images.githubusercontent.com/121365233/224875308-378403c0-0099-448a-ad27-ea9cb55730e4.png">

--Following the same path create "outputs.tf" file.

<img width="316" alt="Screenshot 2023-03-13 at 10 16 43 PM" src="https://user-images.githubusercontent.com/121365233/224875625-ae1af8c3-106e-4a14-84a0-f6d64e0389a5.png">

<img width="366" alt="Screenshot 2023-03-13 at 10 17 45 PM" src="https://user-images.githubusercontent.com/121365233/224875691-4311957d-de88-4e5c-9d13-8cd085969b0a.png">

--Now let’s list our files.

<img width="333" alt="Screenshot 2023-03-13 at 10 20 51 PM" src="https://user-images.githubusercontent.com/121365233/224876211-29dfcc46-300d-4d54-bd20-6bbd13c024fc.png">

Congratulations! Now we have created our module!

--NOw we will go back to the main terraform project directory to start writing our main code, which is going to use this module!

<img width="391" alt="Screenshot 2023-03-13 at 10 25 05 PM" src="https://user-images.githubusercontent.com/121365233/224876832-a55cc3b5-372f-4b4e-ab2c-f7f9bd2ab0ef.png">

-- inside our main directory, we will create a file called "main.tf".

<img width="407" alt="Screenshot 2023-03-13 at 10 28 34 PM" src="https://user-images.githubusercontent.com/121365233/224877301-884c4f83-f197-4612-a5a2-e3232829f52b.png">

--paste the code

<img width="373" alt="Screenshot 2023-03-13 at 10 30 14 PM" src="https://user-images.githubusercontent.com/121365233/224877524-bd7ed0f5-518c-4804-af28-b28239c88444.png">

--Before we invoke terraform code that we have written, let’s create on more "outputs.tf" file inside our main directory.

<img width="433" alt="Screenshot 2023-03-13 at 10 33 08 PM" src="https://user-images.githubusercontent.com/121365233/224877981-4dfd8462-b42b-4356-a55d-c97d379bab53.png">

<img width="449" alt="Screenshot 2023-03-13 at 10 33 29 PM" src="https://user-images.githubusercontent.com/121365233/224877993-6553d99a-2d06-4d7e-bffd-510a6b464b9b.png">

--And finally run few terraform commands to format the code, look at the plan or review of the deployment and finnaly apply the code.
--So, to format the code, we will be using command terraform format.
--And we will be passing recursive flag so that this command go inside subfolders of this main project folder and format all the terraform code files.

<img width="719" alt="Screenshot 2023-03-13 at 10 40 30 PM" src="https://user-images.githubusercontent.com/121365233/224878926-885af413-32c8-49c0-abc4-640fe0d4bf36.png">

--terraform validate command check and makes us sure that we are not having any wrong syntaxes.

<img width="458" alt="Screenshot 2023-03-13 at 10 42 41 PM" src="https://user-images.githubusercontent.com/121365233/224879341-5d1df2de-34a6-445d-bead-fac7cb476556.png">

--To take a review of our project before we deploy it.

<img width="1170" alt="Screenshot 2023-03-13 at 10 44 52 PM" src="https://user-images.githubusercontent.com/121365233/224879664-47168235-5cd5-4820-af21-c5fcc6cd0bcd.png">

<img width="1166" alt="Screenshot 2023-03-13 at 10 46 25 PM" src="https://user-images.githubusercontent.com/121365233/224879950-7df546d8-ca4a-48de-9ac3-7993a550bf78.png">

<img width="707" alt="Screenshot 2023-03-13 at 10 50 58 PM" src="https://user-images.githubusercontent.com/121365233/224880617-09825a36-d4c2-46c0-96d2-43ecc2b73134.png">

--As you can see our three resources used module.

<img width="499" alt="Screenshot 2023-03-13 at 10 52 38 PM" src="https://user-images.githubusercontent.com/121365233/224880977-455c0d6a-4b92-4a8a-ad8d-2048726d4f6f.png">

Finally, don’t forget destroying your resources before you close the lab.

<img width="1124" alt="Screenshot 2023-03-13 at 10 57 00 PM" src="https://user-images.githubusercontent.com/121365233/224881559-13a5837c-1c3e-450e-8413-f92cb6bb729c.png">





