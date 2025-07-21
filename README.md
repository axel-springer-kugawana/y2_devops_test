# Home Exercise
• The purpose of the following tasks is to gain familiarity with your way of thinking, your approach to new problems, and your ability to design and implement cloud solutions.

• Please spend only as much time as you are able and willing to in order to finish the exercises as efficiently as possible. Don't be concerned with minor elements that you believe are irrelevant to the exercise; but, keep in mind that we want to see efficient, readable, and well-designed code.

• You can provide an architecture document or complement your code with comments to help us understand why you chose to implement things the way you did.

• Please implement with AWS cloud vendor


## **Exercise**:

Design and implement an environment with an EKS cluster.

The running service should be this simple go web application containerized.

### **Task 1 - IaC**
Create all of the neccessry cloud resorces in order to build the EKS cluster using Terraform.
### **Task 2 - Dockerize**
Create a `Dockerfile` for this simple go web application.

### **Task 3 - Kubernetes Integration**
Create all of the neccessry objects in order to run the application in a working kubernetes cluster.

### **Task 4 - CI/CD Pipeline**

#### GitHub Actions
Create a GitHub Actions workflow in `.github/workflows/` with:
* Proper environment secrets configuration
* Workflow triggers on push/PR
* Build docker image
* Tag the new image as `<branch_name>-<sha>`
* Test the image before pushing (validate `/posts` endpoint with GET request)
* Push image to container registry
* Deploy to EKS cluster

Choose the approach that best fits your workflow needs.

## **Submissions:**
1. Link to a git repository with the source code and any other relevant and
supporting information.
2. Screenshots of the following:
    1. Running cluster instance in AWS console
    2. Running pods

