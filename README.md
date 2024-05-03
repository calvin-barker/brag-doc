# Brag Doc 
Inspired by https://jvns.ca/blog/brag-documents/

## Prereqs
Install https://github.com/bovem/brag

```sh
# Set up the brag CLI
gh repo clone calvin-barker/brag
cd brag
go build
sudo mv ./brag /usr/local/bin
sudo chmod +x /usr/local/bin/brag

# Configure the brag doc location
cd ../brag-doc
echo "export BRAG_DOCS_LOC=$(pwd)/work-docs" >> ~/.zshrc
echo "export BRAG_DOCS_REPO_SYNC=true" >> ~/.zshrc
source ~/.zshrc
brag init

# Start bragging
brag -c "Setup brag on a new computer"

```
