# About

Sun Energy is committed to revolutionizing blockchain validation by emphasizing sustainability at the core of its operations. We are dedicated to empowering blockchain networks with dependable and eco-conscious practices, ensuring their seamless and efficient functioning. Our focus lies in offering sustainable solutions for blockchain validation, setting a new standard for reliable and environmentally responsible operations.

# Projects

As active participants in the **0G Labs**, Sun Energy is deeply involved in setting up and maintaining nodes to bolster secure and dependable network operations. We are committed to supporting 0G’s vision of establishing a decentralized and eco-friendly blockchain network, aligning with our core values of sustainability and reliability.
```
git clone https://github.com/0glabs/0g-node.git
cd 0g-node

npm install

echo '{
  "validator": {
    "name": "Syn Energy",
    "evm_address": "synenergy-evm"
  },
  "network": {
    "rpc_url": "https://rpc-testnet.0g.ai",
    "chain_id": 16600
  },
  "node": {
    "private_key": "YOUR_PRIVATE_KEY",
    "ip": "0.0.0.0",
    "port": 30303
  }
}' > config.json

npm start -- --config ./config.json

echo 'FROM node:14

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./

RUN npm install

# Bundle app source
COPY . .

EXPOSE 30303

CMD [ "npm", "start", "--", "--config", "./config.json" ]' > Dockerfile

docker build -t 0g-node .

docker run -d --name 0g-node -p 30303:30303 0g-node
```

In the context of the **Symbiotic** project, Sun Energy offers valuable node validation services aimed at enhancing network efficiency and security. Leveraging our expertise, we focus on monitoring and optimization efforts to contribute to the stability and overall performance of the network, ensuring that it operates at its best while prioritizing sustainability.
```
git clone https://github.com/symbioticfi/symbiotic-node.git
cd symbiotic-node

# Step 2: Install dependencies
npm install

# Step 3: Create the configuration file
echo '{
  "validator": {
    "name": "synenergy",
    "evm_address": "synenergy-evm"
  },
  "network": {
    "rpc_url": "https://rpc.symbiotic.fi",
    "chain_id": 2024
  },
  "node": {
    "private_key": "YOUR_PRIVATE_KEY",
    "ip": "0.0.0.0",
    "port": 30303
  }
}' > config.json

# Step 4: Start the node
npm start -- --config ./config.json

# Step 5: (Optional) Docker setup
# Create a Dockerfile
echo 'FROM node:14
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 30303
CMD [ "npm", "start", "--", "--config", "./config.json" ]
' > Dockerfile

# Build the Docker image
docker build -t symbiotic-node .

# Run the Docker container
docker run -d --name symbiotic-node -p 30303:30303 symbiotic-node

# Step 6: Check logs (optional)
docker logs -f symbiotic-node
```

Within the **Airchains** project, Sun Energy plays a crucial role in deploying and maintaining nodes to uphold a secure and high-performing blockchain network. Our dedicated focus on security audits and performance optimization empowers the network to operate seamlessly, in line with our commitment to ensuring responsible and efficient blockchain operations.
```
In the pending
```

**Nubit** In the pending
```
In the pending
```

# More Info/Contacts

Gitbook: https://sun-energy.gitbook.io/sun-energy/projects

Keybase: https://keybase.io/sunvalidator

Twitter: https://twitter.com/sunvalidator

Discord: sunvalidator
