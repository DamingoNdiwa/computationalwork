# computationalwork

* a modified version of this file README.md file containing the specific commands that you used to complete the exercises. You do not have to include everything, just the key commands. 
* A wallet.py file that passes the unit tests.
* A Dockerfile.

# Dockerfile

touch Douckerfile
# Build and push Docker image

docker build -t damingondiwa/computational-workflows .
docker login 
docker push

# Run a container, and share in files from the host.

docker run -ti -v $(pwd):/root/shared damingondiwa/computational-workflows:latest

# Setup a simple Python test suite

* Start a Docker container using your image and share your repository into a directory /root/shared into the container.

docker run -ti -v $(pwd):/root/shared damingondiwa/computational-workflows

* Run the tests inside the container by going to /root/shared and running the command py.test-3. The tests should fail.


cd /root/shared 

pytest-3







