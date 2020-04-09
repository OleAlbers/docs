
---
title: "ClusterAlterRule"
block_external_search_index: true
---






## Create a ClusterAlterRule Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterAlterRule">ClusterAlterRule</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterAlterRuleArgs">ClusterAlterRuleArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">ClusterAlterRule</span><span class="p">(resource_name, opts=None, </span>annotations=None<span class="p">, </span>cluster_id=None<span class="p">, </span>event_rule=None<span class="p">, </span>group_id=None<span class="p">, </span>group_interval_seconds=None<span class="p">, </span>group_wait_seconds=None<span class="p">, </span>inherited=None<span class="p">, </span>labels=None<span class="p">, </span>metric_rule=None<span class="p">, </span>name=None<span class="p">, </span>node_rule=None<span class="p">, </span>repeat_interval_seconds=None<span class="p">, </span>severity=None<span class="p">, </span>system_service_rule=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewClusterAlterRule<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleArgs">ClusterAlterRuleArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRule">ClusterAlterRule</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ClusterAlterRule.html">ClusterAlterRule</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.ClusterAlterRuleArgs.html">ClusterAlterRuleArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>System<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">*Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">*Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">*Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>System<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">*Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>system<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>event_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>group_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>wait_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>node_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>system_<wbr>service_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## ClusterAlterRule Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>System<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">*Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">*Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">*Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>System<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">*Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>system<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>event_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group_<wbr>wait_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>metric_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>node_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>repeat_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>system_<wbr>service_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing ClusterAlterRule Resource

Get an existing ClusterAlterRule resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterAlterRuleState">ClusterAlterRuleState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ClusterAlterRule">ClusterAlterRule</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>annotations=None<span class="p">, </span>cluster_id=None<span class="p">, </span>event_rule=None<span class="p">, </span>group_id=None<span class="p">, </span>group_interval_seconds=None<span class="p">, </span>group_wait_seconds=None<span class="p">, </span>inherited=None<span class="p">, </span>labels=None<span class="p">, </span>metric_rule=None<span class="p">, </span>name=None<span class="p">, </span>node_rule=None<span class="p">, </span>repeat_interval_seconds=None<span class="p">, </span>severity=None<span class="p">, </span>system_service_rule=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetClusterAlterRule<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleState">ClusterAlterRuleState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRule">ClusterAlterRule</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ClusterAlterRule.html">ClusterAlterRule</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ClusterAlterRuleState.html">ClusterAlterRuleState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>System<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">*Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">*Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">*Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>System<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">*Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cluster<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>event<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>node<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>system<wbr>Service<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
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
    <dd>{{% md %}}The cluster alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cluster_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster id where create cluster alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>event_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterruleeventrule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule event rule. ConflictsWith: `"metric_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>wait_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulemetricrule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule metric rule. ConflictsWith: `"event_rule", "node_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>node_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulenoderule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule node rule. ConflictsWith: `"event_rule", "metric_rule", "system_service_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The cluster alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>system_<wbr>service_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#clusteralterrulesystemservicerule">Dict[Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The cluster alert rule system service rule. ConflictsWith: `"event_rule", "metric_rule", "node_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Cluster<wbr>Alter<wbr>Rule<wbr>Event<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterAlterRuleEventRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterAlterRuleEventRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleEventRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleEventRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Event<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Event type. Supported values : `"Warning" | "Normal"`. Default: `Warning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Resource<wbr>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource kind. Supported values : `"DaemonSet" | "Deployment" | "Node" | "Pod" | "StatefulSet"` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Event<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Event type. Supported values : `"Warning" | "Normal"`. Default: `Warning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Resource<wbr>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource kind. Supported values : `"DaemonSet" | "Deployment" | "Node" | "Pod" | "StatefulSet"` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>event<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Event type. Supported values : `"Warning" | "Normal"`. Default: `Warning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>resource<wbr>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Resource kind. Supported values : `"DaemonSet" | "Deployment" | "Node" | "Pod" | "StatefulSet"` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>event<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Event type. Supported values : `"Warning" | "Normal"`. Default: `Warning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>resource<wbr>Kind</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Resource kind. Supported values : `"DaemonSet" | "Deployment" | "Node" | "Pod" | "StatefulSet"` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Alter<wbr>Rule<wbr>Metric<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterAlterRuleMetricRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterAlterRuleMetricRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleMetricRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleMetricRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">double</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">float64</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Alter<wbr>Rule<wbr>Node<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterAlterRuleNodeRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterAlterRuleNodeRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleNodeRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleNodeRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cpu<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Node rule cpu threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Mem<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Node rule mem threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Node<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Node ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}Node rule selector (map)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Cpu<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Node rule cpu threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Mem<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Node rule mem threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Node<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Node ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Node rule selector (map)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cpu<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Node rule cpu threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>mem<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Node rule mem threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>node<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Node ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}Node rule selector (map)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>cpu<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Node rule cpu threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>mem<wbr>Threshold</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Node rule mem threshold. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>node<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Node ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Node rule selector (map)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Cluster<wbr>Alter<wbr>Rule<wbr>System<wbr>Service<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ClusterAlterRuleSystemServiceRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ClusterAlterRuleSystemServiceRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleSystemServiceRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ClusterAlterRuleSystemServiceRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}System service rule condition. Supported values : `"controller-manager" | "etcd" | "scheduler"`. Default: `scheduler` (string)
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
