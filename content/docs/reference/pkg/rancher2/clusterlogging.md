
---
title: "ClusterLogging"
block_external_search_index: true
---



Provides a Rancher v2 Cluster Logging resource. This can be used to configure Cluster Logging for Rancher v2 environments and retrieve their information.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as rancher2 from "@pulumi/rancher2";

// Create a new Rancher2 Cluster Logging
const foo = new rancher2.ClusterLogging("foo", {
    clusterId: "<cluster_id>",
    kind: "syslog",
    syslogConfig: {
        endpoint: "<syslog_endpoint>",
        protocol: "udp",
        severity: "notice",
        sslVerify: false,
    },
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-rancher2/blob/master/website/docs/r/clusterLogging.html.markdown.



## Create a ClusterLogging Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterLogging">ClusterLogging</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterLoggingArgs">ClusterLoggingArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">ClusterLogging</span><span class="p">(resource_name, opts=None, </span>annotations=None<span class="p">, </span>cluster_id=None<span class="p">, </span>custom_target_config=None<span class="p">, </span>elasticsearch_config=None<span class="p">, </span>enable_json_parsing=None<span class="p">, </span>fluentd_config=None<span class="p">, </span>kafka_config=None<span class="p">, </span>kind=None<span class="p">, </span>labels=None<span class="p">, </span>name=None<span class="p">, </span>namespace_id=None<span class="p">, </span>output_flush_interval=None<span class="p">, </span>output_tags=None<span class="p">, </span>splunk_config=None<span class="p">, </span>syslog_config=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewClusterLogging<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingArgs">ClusterLoggingArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLogging">ClusterLogging</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ClusterLogging.html">ClusterLogging</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.ClusterLoggingArgs.html">ClusterLoggingArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Cluster<wbr>Logging<wbr>Kafka<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Cluster<wbr>Logging<wbr>Splunk<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Cluster<wbr>Logging<wbr>Syslog<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">*Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">*Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">*Cluster<wbr>Logging<wbr>Fluentd<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">*Cluster<wbr>Logging<wbr>Kafka<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">*Cluster<wbr>Logging<wbr>Splunk<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">*Cluster<wbr>Logging<wbr>Syslog<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Cluster<wbr>Logging<wbr>Kafka<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Cluster<wbr>Logging<wbr>Splunk<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Cluster<wbr>Logging<wbr>Syslog<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>custom_<wbr>target_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Dict[Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>elasticsearch_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Dict[Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable_<wbr>json_<wbr>parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fluentd_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Dict[Cluster<wbr>Logging<wbr>Fluentd<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>kafka_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Dict[Cluster<wbr>Logging<wbr>Kafka<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>namespace_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output_<wbr>flush_<wbr>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output_<wbr>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>splunk_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Dict[Cluster<wbr>Logging<wbr>Splunk<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>syslog_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Dict[Cluster<wbr>Logging<wbr>Syslog<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## ClusterLogging Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Cluster<wbr>Logging<wbr>Kafka<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Cluster<wbr>Logging<wbr>Splunk<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Cluster<wbr>Logging<wbr>Syslog<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">*Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">*Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">*Cluster<wbr>Logging<wbr>Fluentd<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">*Cluster<wbr>Logging<wbr>Kafka<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">*Cluster<wbr>Logging<wbr>Splunk<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">*Cluster<wbr>Logging<wbr>Syslog<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Cluster<wbr>Logging<wbr>Kafka<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Cluster<wbr>Logging<wbr>Splunk<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Cluster<wbr>Logging<wbr>Syslog<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>custom_<wbr>target_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Dict[Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>elasticsearch_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Dict[Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>enable_<wbr>json_<wbr>parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>fluentd_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Dict[Cluster<wbr>Logging<wbr>Fluentd<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>kafka_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Dict[Cluster<wbr>Logging<wbr>Kafka<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>namespace_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>output_<wbr>flush_<wbr>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>output_<wbr>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>splunk_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Dict[Cluster<wbr>Logging<wbr>Splunk<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>syslog_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Dict[Cluster<wbr>Logging<wbr>Syslog<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing ClusterLogging Resource

Get an existing ClusterLogging resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterLoggingState">ClusterLoggingState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterLogging">ClusterLogging</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>annotations=None<span class="p">, </span>cluster_id=None<span class="p">, </span>custom_target_config=None<span class="p">, </span>elasticsearch_config=None<span class="p">, </span>enable_json_parsing=None<span class="p">, </span>fluentd_config=None<span class="p">, </span>kafka_config=None<span class="p">, </span>kind=None<span class="p">, </span>labels=None<span class="p">, </span>name=None<span class="p">, </span>namespace_id=None<span class="p">, </span>output_flush_interval=None<span class="p">, </span>output_tags=None<span class="p">, </span>splunk_config=None<span class="p">, </span>syslog_config=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetClusterLogging<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingState">ClusterLoggingState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLogging">ClusterLogging</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ClusterLogging.html">ClusterLogging</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ClusterLoggingState.html">ClusterLoggingState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Cluster<wbr>Logging<wbr>Kafka<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Cluster<wbr>Logging<wbr>Splunk<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Cluster<wbr>Logging<wbr>Syslog<wbr>Config<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">*Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">*Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">*Cluster<wbr>Logging<wbr>Fluentd<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">*Cluster<wbr>Logging<wbr>Kafka<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">*Cluster<wbr>Logging<wbr>Splunk<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">*Cluster<wbr>Logging<wbr>Syslog<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>custom<wbr>Target<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>elasticsearch<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable<wbr>Json<wbr>Parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fluentd<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>kafka<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Cluster<wbr>Logging<wbr>Kafka<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>namespace<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output<wbr>Flush<wbr>Interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output<wbr>Tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>splunk<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Cluster<wbr>Logging<wbr>Splunk<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>syslog<wbr>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Cluster<wbr>Logging<wbr>Syslog<wbr>Config?</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Annotations for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id to configure logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>custom_<wbr>target_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingcustomtargetconfig">Dict[Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The custom target config for Cluster Logging. For `kind = custom`. Conflicts with `elasticsearch_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>elasticsearch_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingelasticsearchconfig">Dict[Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The elasticsearch config for Cluster Logging. For `kind = elasticsearch`. Conflicts with `custom_target_config`, `fluentd_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable_<wbr>json_<wbr>parsing</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enable json log parsing. Default: `false` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fluentd_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfig">Dict[Cluster<wbr>Logging<wbr>Fluentd<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The fluentd config for Cluster Logging. For `kind = fluentd`. Conflicts with `custom_target_config`, `elasticsearch_config`, `kafka_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>kafka_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingkafkaconfig">Dict[Cluster<wbr>Logging<wbr>Kafka<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The kafka config for Cluster Logging. For `kind = kafka`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `splunk_config` and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The kind of the Cluster Logging. `elasticsearch`, `fluentd`, `kafka`, `splunk` and `syslog` are supported (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Labels for Cluster Logging object (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The name of the cluster logging config (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>namespace_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The namespace id from cluster logging (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output_<wbr>flush_<wbr>interval</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}How often buffered logs would be flushed. Default: `3` seconds (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>output_<wbr>tags</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The output tags for Cluster Logging (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>splunk_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsplunkconfig">Dict[Cluster<wbr>Logging<wbr>Splunk<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The splunk config for Cluster Logging. For `kind = splunk`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `syslog_config` (list maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>syslog_<wbr>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingsyslogconfig">Dict[Cluster<wbr>Logging<wbr>Syslog<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}The syslog config for Cluster Logging. For `kind = syslog`. Conflicts with `custom_target_config`, `elasticsearch_config`, `fluentd_config`, `kafka_config`, and `splunk_config` (list maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Cluster<wbr>Logging<wbr>Custom<wbr>Target<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingCustomTargetConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingCustomTargetConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingCustomTargetConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingCustomTargetConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Content</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Custom target config content (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Content</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Custom target config content (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>content</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Custom target config content (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>content</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Custom target config content (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Logging<wbr>Elasticsearch<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingElasticsearchConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingElasticsearchConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingElasticsearchConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingElasticsearchConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}User password for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Username for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Date<wbr>Format</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Date format for the elascticsearch logs. Default: `YYYY-MM-DD` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Index<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Index prefix for the elascticsearch logs. Default: `local` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL version for the elascticsearch service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}User password for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Auth<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Username for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Date<wbr>Format</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Date format for the elascticsearch logs. Default: `YYYY-MM-DD` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Index<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Index prefix for the elascticsearch logs. Default: `local` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL version for the elascticsearch service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>auth<wbr>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}User password for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>auth<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Username for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>date<wbr>Format</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Date format for the elascticsearch logs. Default: `YYYY-MM-DD` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>index<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Index prefix for the elascticsearch logs. Default: `local` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL version for the elascticsearch service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>auth<wbr>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}User password for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>auth<wbr>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Username for the elascticsearch service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>date<wbr>Format</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Date format for the elascticsearch logs. Default: `YYYY-MM-DD` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>index<wbr>Prefix</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Index prefix for the elascticsearch logs. Default: `local` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL version for the elascticsearch service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Logging<wbr>Fluentd<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingFluentdConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingFluentdConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingFluentdConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingFluentdConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Compress</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Compress data for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Tls</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Enable TLS for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Fluent<wbr>Servers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfigfluentserver">List&lt;Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Fluent<wbr>Server<wbr>Args&gt;</a></span>
    </dt>
    <dd>{{% md %}}Servers for the fluentd service (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Compress</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Compress data for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Enable<wbr>Tls</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Enable TLS for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Fluent<wbr>Servers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfigfluentserver">[]Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Fluent<wbr>Server</a></span>
    </dt>
    <dd>{{% md %}}Servers for the fluentd service (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>compress</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Compress data for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable<wbr>Tls</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Enable TLS for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>fluent<wbr>Servers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfigfluentserver">Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Fluent<wbr>Server[]</a></span>
    </dt>
    <dd>{{% md %}}Servers for the fluentd service (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>compress</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Compress data for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>enable<wbr>Tls</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Enable TLS for the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>fluent<wbr>Servers</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusterloggingfluentdconfigfluentserver">List[Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Fluent<wbr>Server]</a></span>
    </dt>
    <dd>{{% md %}}Servers for the fluentd service (list)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Logging<wbr>Fluentd<wbr>Config<wbr>Fluent<wbr>Server</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingFluentdConfigFluentServer">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingFluentdConfigFluentServer">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingFluentdConfigFluentServerArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingFluentdConfigFluentServerOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Hostname</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Hostname of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}User password of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Shared<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Shared key of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Standby</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}Standby server of the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Username of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Weight</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Weight of the fluentd server (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Hostname</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Hostname of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}User password of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Shared<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Shared key of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Standby</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}Standby server of the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Username</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Username of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Weight</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Weight of the fluentd server (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>hostname</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Hostname of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}User password of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>shared<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Shared key of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>standby</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}Standby server of the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>username</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Username of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>weight</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Weight of the fluentd server (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>hostname</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Hostname of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}User password of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>shared<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Shared key of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>standby</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}Standby server of the fluentd service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>username</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Username of the fluentd service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>weight</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Weight of the fluentd server (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Logging<wbr>Kafka<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingKafkaConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingKafkaConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingKafkaConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingKafkaConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Broker<wbr>Endpoints</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}Kafka endpoints for kafka service. Conflicts with `zookeeper_endpoint` (list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Topic</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Topic to publish on the kafka service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Zookeeper<wbr>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Zookeeper endpoint for kafka service. Conflicts with `broker_endpoints` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Broker<wbr>Endpoints</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}Kafka endpoints for kafka service. Conflicts with `zookeeper_endpoint` (list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Topic</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Topic to publish on the kafka service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Zookeeper<wbr>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Zookeeper endpoint for kafka service. Conflicts with `broker_endpoints` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>broker<wbr>Endpoints</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}Kafka endpoints for kafka service. Conflicts with `zookeeper_endpoint` (list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>topic</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Topic to publish on the kafka service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>zookeeper<wbr>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Zookeeper endpoint for kafka service. Conflicts with `broker_endpoints` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>broker<wbr>Endpoints</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}Kafka endpoints for kafka service. Conflicts with `zookeeper_endpoint` (list)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>topic</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Topic to publish on the kafka service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>zookeeper<wbr>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Zookeeper endpoint for kafka service. Conflicts with `broker_endpoints` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Logging<wbr>Splunk<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingSplunkConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingSplunkConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingSplunkConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingSplunkConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Index</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Index prefix for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Source</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Date format for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Index</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Index prefix for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Source</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Date format for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>index</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Index prefix for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>source</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Date format for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key<wbr>Pass</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key password for the splunk service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>index</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Index prefix for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>source</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Date format for the splunk logs (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Logging<wbr>Syslog<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterLoggingSyslogConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterLoggingSyslogConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingSyslogConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterLoggingSyslogConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Program</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Program for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Protocol for the syslog service. `tcp` and `udp` are supported. Default: `udp` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Date format for the syslog logs. `emergency`, `alert`, `critical`, `error`, `warning`, `notice`, `info` and `debug` are supported. Default: `notice` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Program</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Program for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Protocol for the syslog service. `tcp` and `udp` are supported. Default: `udp` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Date format for the syslog logs. `emergency`, `alert`, `critical`, `error`, `warning`, `notice`, `info` and `debug` are supported. Default: `notice` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Token</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>program</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Program for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Protocol for the syslog service. `tcp` and `udp` are supported. Default: `udp` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Date format for the syslog logs. `emergency`, `alert`, `critical`, `error`, `warning`, `notice`, `info` and `debug` are supported. Default: `notice` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>certificate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Cert</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client certificate for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>client<wbr>Key</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}SSL client key for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>endpoint</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Endpoint of the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>program</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Program for the syslog service (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>protocol</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Protocol for the syslog service. `tcp` and `udp` are supported. Default: `udp` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Date format for the syslog logs. `emergency`, `alert`, `critical`, `error`, `warning`, `notice`, `info` and `debug` are supported. Default: `notice` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>ssl<wbr>Verify</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}SSL verify for the syslog service (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>token</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Token for the syslog service (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-rancher2">https://github.com/pulumi/pulumi-rancher2</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
