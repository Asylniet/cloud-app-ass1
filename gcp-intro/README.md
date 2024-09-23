# 1. What is the default home directory in Cloud Shell?
/home/assylniyet
# 2. What tools are pre-installed in Cloud Shell?
 - git
 - gcloud
 - python
 - docker
 - npm/node
 - postgresql
 - and many more like go, ruby, c++, etc.
# 3. How can you open the built-in code editor in Cloud Shell?
I guess, there should be code command supported, but I couldn't run it on mine.
I used nano instead.


---

# 1. How do you list all projects associated with your account?
gcloud projects list
# 2. What command is used to set a default project?
gcloud config set project <project-id>
# 3. How do you describe project metadata?
gcloud projects describe <project-id>

---

# 1. What command did you use to create the directory structure?
mkdir -p ~/{gcp-intro,gcp-intro/gcp-intro-1,gcp-intro/gcp-intro-2}
# 2. How did you upload a file to a Cloud Storage bucket?
gsutil cp ~/gcp-intro/gcp-intro-1/README.md gs://gcp-intro-1
# 3. How can you list the contents of a Cloud Storage bucket?
gsutil ls gs://gcp-intro-1

---

# 1. What command did you use to make the script executable?
chmod +x ~/gcp-intro/gcp-intro-1/gcp-intro-1.sh
# 2. How did you ensure the script was executed correctly?
./gcp-intro-1.sh
# 3. What steps did your script automate?
    - Create a Cloud Storage bucket
    - Upload a file to the bucket
    - List the contents of the bucket
    - Delete the bucket
