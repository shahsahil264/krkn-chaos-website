---
title: krkn-chaos
linkTitle: "Krkn Chaos"
---

{{< blocks/cover title="Krkn - Chaos and resiliency testing tool for Kubernetes" image_anchor="top" height="full" >}}
<img class="w-25 mb-4" src="img/2024_krkn_logo__Krkn_Full.svg" alt="Krkn logo" />
<a class="btn btn-lg btn-primary me-3 mb-4" href="/docs/">
  Documentation <i class="fas fa-arrow-alt-circle-right ms-2"></i>
</a>
<a class="btn btn-lg btn-secondary me-3 mb-4" href="https://github.com/krkn-chaos">
  Github <i class="fab fa-github ms-2 "></i>
</a>
<p class="lead mt-5">Unleash Chaos, Ensure Resilience!  
Make Kubernetes Sweat -Unleash the Kraken!</p>
{{< blocks/link-down color="info" >}}
{{< /blocks/cover >}}


{{% blocks/lead color="primary" %}}
Krkn aka **Kraken** is a chaos and resiliency testing tool for Kubernetes. Kraken injects deliberate **failures** into Kubernetes clusters to check if it is resilient to turbulent conditions.
{{% /blocks/lead %}}


{{% blocks/section color="dark" type="row" %}}

{{% blocks/feature icon="fa-solid fa-magnifying-glass" %}}
Watches for the presence of a reboot sentinel file e.g. `/var/run/reboot-required`
or the successful run of a sentinel command.
{{% /blocks/feature %}}

{{% blocks/feature icon="fa-solid fa-lock" %}}
Utilises a lock in the API server to ensure only one node reboots at a time.
{{% /blocks/feature %}}

{{% blocks/feature icon="fa-solid fa-user-clock" %}}
Optionally defers reboots in the presence of active Prometheus alerts or selected pods.
{{% /blocks/feature %}}

{{% blocks/feature icon="fa-solid fa-list-check" %}}
Cordons & drains worker nodes before reboot, uncordoning them after.
{{% /blocks/feature %}}

<!-- {{% blocks/feature icon="fab fa-github" title="Contributions welcome!" url="https://github.com/google/docsy-example" %}}
We do a [Pull Request](https://github.com/google/docsy-example/pulls) contributions workflow on **GitHub**. New users are always welcome!
{{% /blocks/feature %}} -->

{{< /blocks/section >}}

{{< blocks/section color="white" >}}

  <div class="container">
    <div class="row">
      <img src="/img/cncf-color.png" width="600px" class="cncf-logo img-fluid mb-3">
    </div>
    <div class="row">
      <p class="text-muted">Krkn is a Cloud Native Computing Foundation Sandbox project.</p>
    </div>
    <div class="row">
      <small class="text-muted">The Linux Foundation® (TLF) has registered trademarks and uses trademarks. For a list of TLF trademarks, see <a href="https://www.linuxfoundation.org/trademark-usage/">Trademark Usage</a>.</small>
    </div>
  </div>

{{< /blocks/section >}}