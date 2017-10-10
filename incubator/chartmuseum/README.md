# ChartMuseum Helm Chart

Work in progress...

Please see https://github.com/chartmuseum/chartmuseum

# For Fleet Devs

* `cd ...kubernetes/charts/incubabator/chartmuseum`
* Create `gke-credentials.json` file and put the `service_account` credentials JSON object in it
* `helm dependency build`
* `helm install . -n chartmuseum --namespace toto`

Note: if you want to access the chartmuseum from the outside, set `service.type` to `NodePort` in `values.yaml`.
