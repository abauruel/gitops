docker build -t abauruel/gitops:latest .

docker run --rm -p 8080:8080 abauruel/gitops:latest 

docker push abauruel/gitops:latest