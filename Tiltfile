docker_compose('docker-compose.yml')

cmd='sleep 10 && cat kcp/admin.kubeconfig | sed -e \'s;://\\([^/]*\\);://localhost:6443;\' > kcp/localhost.kubeconfig'
local_resource('kubeconfig',cmd,allow_parallel=True)