# INSTRUCTIONS 

## WITH NETWORK SHAPING
For deploying the rigor agent to openshift w/ Network Shaping - 
1. Create a new project or navigate to an existing openshift project
2. Insert your RUNNER_TOKEN environment variable in deployment.yaml
3. Insert your project name (from Step 1) in scc.yaml
4. Apply the files in order - 

```
oc apply -f serviceaccount.yaml
oc apply -f scc.yaml
oc apply -f deployment.yaml
```

## WITHOUT NETWORK SHAPING
For deploying the rigor agent to openshift w/o Network Shaping - 
1. Create a new project or navigate to an existing openshift project
2. Insert your RUNNER_TOKEN environment variable in deployment-no-ns.yaml
3. Insert your project name (from Step 1) in scc-no-ns.yaml
4. Apply the files in order - 

```
oc apply -f serviceaccount.yaml
oc apply -f scc-no-ns.yaml
oc apply -f deployment-no-ns.yaml
```
