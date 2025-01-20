# n8n-nodes-odoo(usable as tool)

![n8n.io - Workflow Automation](https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-logo.png)

Install n8n-nodes-odoo

Try it out

Community nodes

The recommended way to install a node in N8N is using the Community nodes feature.


With docker

Another way is using our docker image Digital Boss' N8N custom nodes docker image. It uses an environment variable to install custom nodes.


Run the node locally

N8N Guide on how to run a node locally


Clone the n8n-nodes-odoo repository and execute:


# Install dependencies
npm install

# Build the code
npm run build

# Create symlink at your global node_modules cache
npm link
ls -la $(npm -g root) # check created link

Create an N8N installation and add the n8n-nodes-odoo to it:


# Create an N8N installation
cd ..
mkdir n8n-local
cd n8n-local
npm init -y
npm install --save-dev n8n

# "Install" the locally published module
npm link {{packageFullName}}

# Start n8n
npx n8n

License
