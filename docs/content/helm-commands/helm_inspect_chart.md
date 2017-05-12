+++
title = "helm inspect chart"
weight = "18"

tags = ["commands"]
section = "helm-commands"
categories = ["helm-commands"]
type = "page"

slug = "helm-inspect-chart"

[menu.main]
  url = "helm-inspect-chart"
  parent = "helm-commands"

+++

## helm inspect chart

shows inspect chart

### Synopsis



This command inspects a chart (directory, file, or URL) and displays the contents
of the Charts.yaml file


```
helm inspect chart [CHART]
```

### Options

```
      --ca-file string     chart repository url where to locate the requested chart
      --cert-file string   verify certificates of HTTPS-enabled servers using this CA bundle
      --key-file string    identify HTTPS client using this SSL key file
      --keyring string     path to the keyring containing public verification keys (default "~/.gnupg/pubring.gpg")
      --repo string        chart repository url where to locate the requested chart
      --verify             verify the provenance data for this chart
      --version string     version of the chart. By default, the newest chart is shown
```

### Options inherited from parent commands

```
      --debug                     enable verbose output
      --home string               location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string               address of tiller. Overrides $HELM_HOST
      --kube-context string       name of the kubeconfig context to use
      --tiller-namespace string   namespace of tiller (default "kube-system")
```

### SEE ALSO
* [helm inspect](#helm-inspect)	 - inspect a chart
