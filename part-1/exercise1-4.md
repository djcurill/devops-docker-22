# Exercise
Start a ubuntu image with the process sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'

# Solution
```bash
docker run -it --rm ubuntu sh -c "apt update; apt install -y curl; echo 'Input website:'; read website; echo 'Searching..'; sleep 1; curl https://$website;"
```