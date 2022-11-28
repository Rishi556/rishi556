Setting up my wireguard: 

- Use https://github.com/angristan/wireguard-install as a base(https://github.com/angristan/wireguard-install/tree/99a199ffa51dbafcfe1c42f94c51b04c336e0404) to be exact, will fork soon to have my own copy
- Get routed subnet, preferabally a /48 to the server(overkill but why not, v6 is awesome). If running on a vm, remember to route to vm addr, not the server addr
- Delete masqurate stuff (`ip6tables -t nat -D POSTROUTING -o eth0 -j MASQUERADE`)
- Check out ip6tables is good (`ip6tables-save`)
- Add firewall(config will be added here soon	™️)
