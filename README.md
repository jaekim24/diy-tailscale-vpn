## Install tailscale (ubuntu)
```  curl -fsSL https://tailscale.com/install.sh | sh ```                                                                       

log into your tailscale account 
``` sudo tailscale up ```

set up remote server as a exit node
``` sudo tailscale set --advertise-exit-node ```

go into the tailscale dashboard and set that server as a exit node
``` TS dash > device settings > edit route settings > enable exit node ```

enable IP forwarding to advertise the device as an exit node
```
echo 'net.ipv4.ip_forward = 1' | sudo tee -a /etc/sysctl.d/99-tailscale.conf
echo 'net.ipv6.conf.all.forwarding = 1' | sudo tee -a /etc/sysctl.d/99-tailscale.conf
sudo sysctl -p /etc/sysctl.d/99-tailscale.conf
```

## Claude code install 
```   curl -fsSL https://claude.ai/install.sh | bash   ```


