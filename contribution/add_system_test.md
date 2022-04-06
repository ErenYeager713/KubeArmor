# System tests

Set up KubeArmor in your Vagrant or Kubernetes environment by following the [Development Guide](https://https://github.com/kubearmor/KubeArmor/blob/main/contribution/development_guide.md)

# 1. Sample System Test

## 1.1. Run 'kubectl proxy' in background

```text
(~vagrant)$ kubectl proxy &
```
## 1.2. Start KubeArmor in a another terminal

```text
(~vagrant/KubeArmor/KubeArmor)$ make run
```

<details>
<summary>Output</summary>

```text
cd /home/vagrant/KubeArmor/KubeArmor; make -C ../protobuf
make[1]: Entering directory '/home/vagrant/KubeArmor/protobuf'
make[1]: Nothing to be done for 'build'.
make[1]: Leaving directory '/home/vagrant/KubeArmor/protobuf'
/home/vagrant/KubeArmor/KubeArmor/patch.sh
go: downloading github.com/iovisor/gobpf v0.2.0
cd /home/vagrant/KubeArmor/KubeArmor; go mod tidy
go: downloading github.com/spf13/viper v1.4.0
go: downloading github.com/containerd/containerd v1.5.2
go: downloading github.com/containerd/typeurl v1.0.2
go: downloading github.com/docker/docker v20.10.7+incompatible
go: downloading github.com/opencontainers/runtime-spec v1.0.3-0.20200929063507-e6143ca7d51d
go: downloading google.golang.org/grpc v1.34.0
go: downloading k8s.io/api v0.21.2
go: downloading k8s.io/apimachinery v0.21.2
go: downloading k8s.io/client-go v0.21.2
go: downloading github.com/google/uuid v1.3.0
go: downloading go.uber.org/zap v1.18.1
go: downloading github.com/fsnotify/fsnotify v1.4.9
go: downloading github.com/hashicorp/hcl v1.0.0
go: downloading github.com/magiconair/properties v1.8.0
go: downloading github.com/mitchellh/mapstructure v1.1.2
go: downloading github.com/pelletier/go-toml v1.8.1
go: downloading github.com/spf13/afero v1.2.2
go: downloading github.com/spf13/cast v1.3.0
go: downloading github.com/spf13/jwalterweatherman v1.0.0
go: downloading github.com/spf13/pflag v1.0.5
go: downloading gopkg.in/yaml.v2 v2.4.0
go: downloading github.com/stretchr/testify v1.7.0
go: downloading github.com/gogo/protobuf v1.3.2
go: downloading github.com/pkg/errors v0.9.1
go: downloading github.com/opencontainers/go-digest v1.0.0
go: downloading github.com/containerd/ttrpc v1.0.2
go: downloading google.golang.org/protobuf v1.27.1
go: downloading golang.org/x/net v0.0.0-20210805182204-aaa1db679c0d
go: downloading github.com/golang/protobuf v1.5.2
go: downloading github.com/docker/go-connections v0.4.0
go: downloading github.com/docker/go-units v0.4.0
go: downloading github.com/opencontainers/image-spec v1.0.1
go: downloading github.com/docker/distribution v2.7.1+incompatible
go: downloading gotest.tools/v3 v3.0.3
go: downloading gotest.tools v2.2.0+incompatible
go: downloading k8s.io/klog/v2 v2.8.0
go: downloading github.com/google/gofuzz v1.2.0
go: downloading sigs.k8s.io/yaml v1.2.0
go: downloading github.com/imdario/mergo v0.3.11
go: downloading golang.org/x/term v0.0.0-20210220032956-6a3ed077a48d
go: downloading github.com/google/go-cmp v0.5.5
go: downloading google.golang.org/genproto v0.0.0-20210108203827-ffc7fda8c3d7
go: downloading go.uber.org/atomic v1.7.0
go: downloading go.uber.org/multierr v1.6.0
go: downloading go.uber.org/goleak v1.1.10
go: downloading github.com/benbjohnson/clock v1.1.0
go: downloading golang.org/x/sys v0.0.0-20210809222454-d867a43fc93e
go: downloading github.com/davecgh/go-spew v1.1.1
go: downloading golang.org/x/text v0.3.6
go: downloading gopkg.in/check.v1 v1.0.0-20200227125254-8fa46927fb4f
go: downloading github.com/pmezard/go-difflib v1.0.0
go: downloading gopkg.in/yaml.v3 v3.0.0-20210107192922-496545a6307b
go: downloading github.com/sirupsen/logrus v1.7.0
go: downloading github.com/prometheus/procfs v0.6.0
go: downloading github.com/Microsoft/go-winio v0.4.17
go: downloading github.com/gorilla/mux v1.8.0
go: downloading sigs.k8s.io/structured-merge-diff/v4 v4.1.0
go: downloading gopkg.in/inf.v0 v0.9.1
go: downloading github.com/json-iterator/go v1.1.10
go: downloading github.com/modern-go/reflect2 v1.0.1
go: downloading github.com/go-logr/logr v0.4.0
go: downloading github.com/googleapis/gnostic v0.4.1
go: downloading golang.org/x/time v0.0.0-20210220033141-f8bda1e9f3ba
go: downloading k8s.io/utils v0.0.0-20201110183641-67b214c5f920
go: downloading golang.org/x/oauth2 v0.0.0-20200107190931-bf48bf16ab8d
go: downloading golang.org/x/lint v0.0.0-20210508222113-6edffad5e616
go: downloading github.com/niemeyer/pretty v0.0.0-20200227124842-a10e7caefd8e
go: downloading github.com/moby/term v0.0.0-20201216013528-df9cb8a40635
go: downloading github.com/morikuni/aec v1.0.0
go: downloading golang.org/x/xerrors v0.0.0-20200804184101-5ec99f83aff1
go: downloading github.com/modern-go/concurrent v0.0.0-20180306012644-bacd9c7ef1dd
go: downloading github.com/kr/text v0.2.0
go: downloading github.com/creack/pty v1.1.11
go: downloading google.golang.org/appengine v1.6.6
go: downloading golang.org/x/tools v0.1.7
go: downloading github.com/Azure/go-ansiterm v0.0.0-20170929234023-d6e3b3328b78
go: downloading golang.org/x/mod v0.4.2
cd /home/vagrant/KubeArmor/KubeArmor; go build -o kubearmor main.go
cd /home/vagrant/KubeArmor/deployments/CRD; kubectl apply -f KubeArmorPolicy.yaml
customresourcedefinition.apiextensions.k8s.io/kubearmorpolicies.security.kubearmor.com created
cd /home/vagrant/KubeArmor/deployments/CRD; kubectl apply -f KubeArmorHostPolicy.yaml
customresourcedefinition.apiextensions.k8s.io/kubearmorhostpolicies.security.kubearmor.com created
cd /home/vagrant/KubeArmor/KubeArmor; sudo rm -f /tmp/kubearmor.log
cd /home/vagrant/KubeArmor/KubeArmor; sudo -E ./kubearmor -logPath=/tmp/kubearmor.log -enableKubeArmorPolicy=true -enableKubeArmorHostPolicy=true
2022-04-06 17:11:20.173159	INFO	config [{Cluster:default Host:kubearmor-dev GRPC:32767 LogPath:/tmp/kubearmor.log SELinuxProfileDir:/tmp/kubearmor.selinux Visibility:process,file,network,capabilities HostVisibility:none Policy:true HostPolicy:true KVMAgent:false K8sEnv:true DefaultFilePosture:block DefaultNetworkPosture:block DefaultCapabilitiesPosture:block CoverageTest:false}]
2022-04-06 17:11:20.197744	INFO	Initialized Kubernetes client
2022-04-06 17:11:20.199101	INFO	Started to monitor node events
2022-04-06 17:11:21.208696	INFO	Initialized KubeArmor Logger
2022-04-06 17:11:21.215584	INFO	Initializing an eBPF program
2022-04-06 17:11:26.707509	INFO	Initialized the eBPF program
2022-04-06 17:11:27.156486	INFO	Initialized KubeArmor Monitor
2022-04-06 17:11:27.156665	INFO	Started to monitor system events
2022-04-06 17:11:27.229163	INFO	Registered the KubeArmor host profile in kubearmor-dev
2022-04-06 17:11:27.229362	INFO	Initialized AppArmor Enforcer
2022-04-06 17:11:27.229404	INFO	Initialized KubeArmor Enforcer
2022-04-06 17:11:27.229446	INFO	Started to protect a host and containers
2022-04-06 17:11:27.229483	INFO	Container Runtime: docker://18.9.1
2022-04-06 17:11:27.251575	INFO	Detected a container (added/2e03b0fe2f85)
2022-04-06 17:11:27.254430	INFO	Detected a container (added/fa4d2ec11340)
2022-04-06 17:11:27.256884	INFO	Detected a container (added/d5bb5b729e39)
2022-04-06 17:11:27.260081	INFO	Detected a container (added/2af6a55698ad)
2022-04-06 17:11:27.262809	INFO	Detected a container (added/ff33531a1843)
2022-04-06 17:11:27.264795	INFO	Detected a container (added/8a6e8a6bbeef)
2022-04-06 17:11:27.266571	INFO	Detected a container (added/c5c070db6952)
2022-04-06 17:11:27.267869	INFO	Detected a container (added/9c59773cd401)
2022-04-06 17:11:27.270235	INFO	Detected a container (added/b71848550a48)
2022-04-06 17:11:27.272069	INFO	Detected a container (added/14572d934700)
2022-04-06 17:11:27.275632	INFO	Detected a container (added/7dd55fb228c9)
2022-04-06 17:11:27.278358	INFO	Detected a container (added/4cdd3d602dd1)
2022-04-06 17:11:27.291626	INFO	Detected a container (added/60211ca24dfd)
2022-04-06 17:11:27.295118	INFO	Detected a container (added/00aed413f427)
2022-04-06 17:11:27.297743	INFO	Detected a container (added/dfb030707ea6)
2022-04-06 17:11:27.305685	INFO	Detected a container (added/95e6d34fa12a)
2022-04-06 17:11:27.308388	INFO	Detected a container (added/b8e653429e84)
2022-04-06 17:11:27.311962	INFO	Detected a container (added/42425280b08f)
2022-04-06 17:11:27.314538	INFO	Detected a container (added/48805020756a)
2022-04-06 17:11:27.317127	INFO	Detected a container (added/5e5c69be4f1e)
2022-04-06 17:11:27.322103	INFO	Detected a container (added/527438c0bad5)
2022-04-06 17:11:27.326530	INFO	Detected a container (added/db298851adca)
2022-04-06 17:11:27.329561	INFO	Detected a container (added/363ee44ffd02)
2022-04-06 17:11:27.332686	INFO	Detected a container (added/70b2e12e7653)
2022-04-06 17:11:27.348849	INFO	Detected a container (added/b6cb7366e06b)
2022-04-06 17:11:27.361390	INFO	Detected a container (added/fdf9ef0f7816)
2022-04-06 17:11:27.364321	INFO	Detected a container (added/4be9bd6d0668)
2022-04-06 17:11:27.372137	INFO	Detected a container (added/ba74c01f6f14)
2022-04-06 17:11:27.372254	INFO	Started to monitor Docker events
2022-04-06 17:11:28.373720	INFO	Started to monitor Pod events
2022-04-06 17:11:28.381554	INFO	Started to monitor security policies
2022-04-06 17:11:28.382075	INFO	Started to monitor per-namespace default posture
2022-04-06 17:11:28.382137	INFO	Started to monitor host security policies
2022-04-06 17:11:28.382163	INFO	Started to serve gRPC-based log feeds
2022-04-06 17:11:28.382196	INFO	Initialized KubeArmor
```
</details>

## 1.3. Start kArmor logs in another terminal

```text
(~vagrant)$ karmor log [flags]
```

<details>
<summary>Starting karmor logs</summary>

```text
gRPC server: localhost:32767
Created a gRPC client (localhost:32767)
Checked the liveness of the gRPC server
Started to watch alerts
```
</details>

## 1.4. Add your pods

You can also add [multiubuntu](https://github.com/KubeArmor/KubeArmor/examples/multiubuntu) pods in this repository

```text
(~vagrant)$ kubectl apply -f KubeArmor/KubeArmor/examples/multiubuntu
```

You can check the status of newly created pods using
```text
(~vagrant)$ kubectl get pods -A
```
Once the pods are running, you can move to the next section

## 1.5. Apply policy

You can create and apply your own policy or use from the available [policies](https://https://github.com/kubearmor/KubeArmor/tree/main/examples/multiubuntu/security-policies)

```text
(~vagrant/KubeArmor)$ kubectl apply -f examples/multiubuntu/security-policies/ksp-group-1-proc-path-block-from-source.yaml
```
This policy is used to block a process from a source path

<details>
<summary>ksp-group-1-proc-path-block-from-source</summary>

```text
apiVersion: security.kubearmor.com/v1
kind: KubeArmorPolicy
metadata:
  name: ksp-group-1-proc-path-block-from-source
  namespace: multiubuntu
spec:
  severity: 5
  message: "block /bin/dash executing /bin/ls"
  selector:
    matchLabels:
      group: group-1
  process:
    matchPaths:
    - path: /bin/ls
      fromSource:
      - path: /bin/dash
  action:
    Block
```
</details>

## 1.6. Test Manually

First we need to enter a container where we can test our policy

```text
(~vagrant/KubeArmor)$ kubectl exec -it ubuntu-1-deployment-5bd4dff469-c5d9q -n multiubuntu -- bash
```




