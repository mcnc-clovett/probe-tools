# Probe-Tools
## _Docker Containers to Probe Your Network_

Each folder contains a seperate tool's Docker Compose file that will stand up that tool in your Docker instance. Here are the tools currently offered:

- Cacti
-- Cacti provides a robust and extensible operational monitoring and fault management framework for users around the world. Is also a complete network graphing solution designed to harness the power of RRDTool's data storage and graphing functionality.
- Smokeping
-- SmokePing is a deluxe latency measurement tool. It can measure, store and display latency, latency distribution and packet loss. SmokePing uses RRDtool to maintain a longterm data-store and to draw pretty graphs, giving up to the minute information on the state of each network connection.
- Uptime Kuma
-- Uptime Kuma is an easy-to-use self-hosted monitoring tool.
- MCNC Speed Test
-- Based on LibreSpeed, this tool is a web-based speed test that does not require Java, Flash or Websockets to function.
- Portainer-CE
-- Irrespective of your industry, orchestration platform, or computing device, Portainer is the most versatile container management software that simplifies your secure adoption of containers with remarkable speed.

## Usage

You may edit each `docker-compose.yml` file to your needs. The `docker-compose.yml` file at the root can be used to start all of the tools at once.

**To start all the tools**, run this command at the root of the repository:
```sh
docker compose up -d
```

**To run each tool independently**, run the following as appropriate:
```sh
docker compose -f ./<tool folder>/docker-compose.yml up -d 
```
