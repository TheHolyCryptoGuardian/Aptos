# Aptos
Aptos is a new, independent project to fulfill our vision of delivering the safest and most production-ready blockchain in the world.

As stated in The Genesis of Aptos, our mission is to create universal and fair access to decentralized assets for billions of people. The web3 stack is vast and rich, from smart contract platforms to developer infrastructure and tooling, wallets, and decentralized applications. Over the coming years, we expect to build and partner with ecosystem participants to improve the entire space. The Aptos journey begins by working with a decentralized community to deploy a safe, scalable, and upgradable smart contract platform.

There are many smart contract platforms deployed in production today — each with their own unique advantages and tradeoffs. We believe that there is a need for a rapidly innovating and adaptable blockchain to serve the needs of billions today and in the future. Our belief is that the user experience needs significant improvement in safety and scalability in order to reach the masses (especially the non-crypto natives). Over the past three years, our team has been able to research and develop innovative ideas (see links below with our numerous publications) and safely deploy them into production environments. Below, we describe a brief overview of our plans and how we will support frequent and rapid upgrades to the network. In the coming months, we will share a series of deep dives and accompanying technical papers on both current and new initiatives toward achieving our goals.

# Commands to install [Aptos node](https://github.com/TheHolyCryptoGuardian/Aptos/blob/main/Node)

Use `wget -q -O aptos_ait3.sh https://raw.githubusercontent.com/TheHolyCryptoGuardian/Aptos/main/Node && chmod +x aptos_ait3.sh && sudo /bin/bash aptos_ait3.sh` to start installing

Use `docker logs -f --tail 100 aptos-validator-1` to check validator node logs.

Use `cd ~/.aptos && docker-compose restart` to restart the node.

Use `cd ~/.aptos && docker-compose stop` to stop the node.

Use `curl 127.0.0.1:9101/metrics 2> /dev/null | grep aptos_state_sync_version` to watch the progress which can be monitored by querying the metrics port.

Use `source ~/.bash_profile` and then
    `cat ~/.aptos/$APTOS_NODENAME.yaml` to get information for filling out the form.

Use `TCP ports: 80, 6180, 6181, 6182, 9101` to open the ports.

Use `cd ~/.aptos && docker-compose down -v` and then
    `rm -rf ~/.aptos /opt/aptos` to delete the node.
