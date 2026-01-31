## Install tailscale (ubuntu)
```  curl -fsSL https://tailscale.com/install.sh | sh ```                                                                       

log into your tailscale account 
``` sudo tailscale up ```

set up remote server as a exit node
``` sudo tailscale set --advertise-exit-node ```

go into the tailscale dashboard and set that server as a exit node
``` TS dash > device settings > edit route settings > enable exit node ```

## Claude code install 
``` curl -fsSL https://cdn.jsdelivr.net/npm/@anthropics/claude-code/install.sh | sh  ```


