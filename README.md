# INSTRUCTIONS 

1. Create a new project or navigate to an existing openshift project
2. Insert your RUNNER_TOKEN environment variable in deployment.yaml
3. Insert your project name (from Step 1) in scc.yaml
4. Apply the files in order - 

```
oc apply -f serviceaccount.yaml
oc apply -f scc.yaml
oc apply -f deployment.yaml
```
