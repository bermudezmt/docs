---
title: Module ecr
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/awsx</a> &gt; ecr

<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#LifecyclePolicy">class LifecyclePolicy</a></li>
<li><a href="#Repository">class Repository</a></li>
<li><a href="#RepositoryImage">class RepositoryImage</a></li>
<li><a href="#buildAndPushImage">function buildAndPushImage</a></li>
<li><a href="#convertToJSON">function convertToJSON</a></li>
<li><a href="#LifecyclePolicyArgs">interface LifecyclePolicyArgs</a></li>
<li><a href="#LifecyclePolicyRule">interface LifecyclePolicyRule</a></li>
<li><a href="#RepositoryArgs">interface RepositoryArgs</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts">ecr/lifecyclePolicy.ts</a> <a href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts">ecr/repository.ts</a> <a href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts">ecr/repositoryImage.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="LifecyclePolicy">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L18">class <b>LifecyclePolicy</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> LifecyclePolicy</pre>
<h3 class="pdoc-member-header" id="LifecyclePolicy-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L18"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> LifecyclePolicy(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, repository: aws.ecr.Repository, args?: <a href='#LifecyclePolicyArgs'>LifecyclePolicyArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ComponentResourceOptions'>pulumi.ComponentResourceOptions</a>)</pre>


Creates a new [LifecyclePolicy] for the given [repository].  If [args] is not provided, then
[getDefaultLifecyclePolicyArgs] will be used to set the default policy for this repo.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-defaultLifecyclePolicyArgs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L34">method <b>defaultLifecyclePolicyArgs</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>defaultLifecyclePolicyArgs(): <a href='#LifecyclePolicyArgs'>LifecyclePolicyArgs</a></pre>


Creates a default lifecycle policy such that at most a single untagged image is retained. All
tagged layers and images will never expire.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/aws/ecr/lifecyclePolicy.d.ts#L80">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: LifecyclePolicyState, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): LifecyclePolicy</pre>


Get an existing LifecyclePolicy resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/aws/ecr/lifecyclePolicy.d.ts#L85">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of LifecyclePolicy.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L187">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-policy">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/aws/ecr/lifecyclePolicy.d.ts#L89">property <b>policy</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>policy: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The policy document. This is a JSON formatted string. See more details about [Policy Parameters](http://docs.aws.amazon.com/AmazonECR/latest/userguide/LifecyclePolicies.html#lifecycle_policy_parameters) in the official AWS docs. For more information about building IAM policy documents with Terraform, see the [AWS IAM Policy Document Guide](https://www.terraform.io/docs/providers/aws/guides/iam-policy-documents.html).

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-registryId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/aws/ecr/lifecyclePolicy.d.ts#L93">property <b>registryId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>registryId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The registry ID where the repository was created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-repository">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/aws/ecr/lifecyclePolicy.d.ts#L97">property <b>repository</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>repository: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of the repository to apply the policy.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicy-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="Repository">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L31">class <b>Repository</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ComponentResource'>ComponentResource</a></pre>
{{% md %}}

A [Repository] represents an [aws.ecr.Repository] along with an associated [LifecyclePolicy]
controlling how images are retained in the repo.

Docker images can be built and pushed to the repo using the [buildAndPushImage] method.  This
will call into the `@pulumi/docker/buildAndPushImage` function using this repo as the appropriate
destination registry.

{{% /md %}}
<h3 class="pdoc-member-header" id="Repository-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L33"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Repository(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#RepositoryArgs'>RepositoryArgs</a>, opts: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ComponentResourceOptions'>pulumi.ComponentResourceOptions</a>)</pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-buildAndPushImage">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L53">method <b>buildAndPushImage</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public </span>buildAndPushImage(pathOrBuild: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | docker.DockerBuild&gt;): OutputInstance&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt; &amp; { ... }</pre>


Builds the docker container specified by [pathOrBuild] and pushes it to this repository.
The result is the unique ID pointing to that pushed image in this repo.  This unique ID
can be passed as the value to `image: repo.buildAndPushImage(...)` in an `ecs.Container`.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L233">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-registerOutputs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L248">method <b>registerOutputs</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>protected </span>registerOutputs(outputs?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Inputs'>Inputs</a> | <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Inputs'>Inputs</a>&gt; | <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Inputs'>Inputs</a>&gt;): <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#void'>void</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-lifecyclePolicy">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L33">property <b>lifecyclePolicy</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>lifecyclePolicy: aws.ecr.LifecyclePolicy | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-repository">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L32">property <b>repository</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>repository: aws.ecr.Repository;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Repository-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="RepositoryImage">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts#L24">class <b>RepositoryImage</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>implements</span> <a href='#ContainerImageProvider'>ContainerImageProvider</a></pre>
{{% md %}}

A simple pair of a [Repository] and a built docker image that was pushed to it.  This can
be passed in as the `image: repoImage` value to an `ecs.Container`.

{{% /md %}}
<h3 class="pdoc-member-header" id="RepositoryImage-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts#L26"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> RepositoryImage(repository: <a href='#Repository'>Repository</a>, image: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;)</pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="RepositoryImage-environment">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts#L34">method <b>environment</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public </span>environment(): <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#never'>never</a></span>[]</pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="RepositoryImage-image">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts#L33">method <b>image</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public </span>image(): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt; | OutputInstance&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;</pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="RepositoryImage-imageValue">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts#L26">property <b>imageValue</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>imageValue: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="RepositoryImage-repository">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repositoryImage.ts#L25">property <b>repository</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>repository: <a href='#Repository'>Repository</a>;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="buildAndPushImage">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L67">function <b>buildAndPushImage</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>buildAndPushImage(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, pathOrBuild: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | docker.DockerBuild&gt;, args?: <a href='#RepositoryArgs'>RepositoryArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ComponentResourceOptions'>pulumi.ComponentResourceOptions</a>): <a href='#RepositoryImage'>RepositoryImage</a></pre>


Creates a new [Repository] (optionally configured using [args]), builds the docker container
specified by [pathOrBuild] and then pushes the built image to the repository.  The result
contains both the Repository created as well as the unique ID referencing the built image in that
repo.  This result type can be passed in as `image: ecr.buildAndPushImage(...)` for an
`ecs.Container`

{{% /md %}}
</div>
<h2 class="pdoc-module-header" id="convertToJSON">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L46">function <b>convertToJSON</b></a>
</h2>
<div class="pdoc-module-contents">
</div>
<h2 class="pdoc-module-header" id="LifecyclePolicyArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L132">interface <b>LifecyclePolicyArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

See https://docs.aws.amazon.com/AmazonECR/latest/userguide/lifecycle_policy_examples.html for
more details.

{{% /md %}}
<h3 class="pdoc-member-header" id="LifecyclePolicyArgs-rules">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L138">property <b>rules</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>rules: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='#LifecyclePolicyRule'>LifecyclePolicyRule</a>&gt;[]&gt;;</pre>
{{% md %}}

Specifies the rules to determine how images should be retired from this repository. Rules are
ordered from lowest priority to highest.  If there is a rule with a `selection` value of
`any`, then it will have the highest priority.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="LifecyclePolicyRule">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L168">interface <b>LifecyclePolicyRule</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The following behaviors hold for these rules:

 * An image is expired by exactly one or zero rules.

 * An image that matches the tagging requirements of a higher priority rule cannot be expired by
   a rule with a lower priority.

 * Rules can never mark images that are marked by higher priority rules, but can still identify
   them as if they haven't been expired.

 * The set of rules must contain a unique set of tag prefixes.

 * Only one rule is allowed to select `untagged` images.

 * Expiration is always ordered by pushed_at_time, and always expires older images before newer
   ones.

 * When using the `tagPrefixList`, an image is successfully matched if all of the tags in the
   `tagPrefixList` value are matched against any of the image's tags.

 * With `maximumNumberOfImages`, images are sorted from youngest to oldest based on
   pushed_at_time and then all images greater than the specified count are expired.

 * With `maximumAgeLimit`, all images whose pushed_at_time is older than the specified number of
   days based on countNumber are expired.

{{% /md %}}
<h3 class="pdoc-member-header" id="LifecyclePolicyRule-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L172">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Describes the purpose of a rule within a lifecycle policy.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicyRule-maximumAgeLimit">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L200">property <b>maximumAgeLimit</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>maximumAgeLimit?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}

The maximum age limit (in days) for your images.  Either [maximumNumberOfImages] or
[maximumAgeLimit] must be provided.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicyRule-maximumNumberOfImages">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L194">property <b>maximumNumberOfImages</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>maximumNumberOfImages?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}

The maximum number of images that you want to retain in your repository.  Either
[maximumNumberOfImages] or [maximumAgeLimit] must be provided.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="LifecyclePolicyRule-selection">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/lifecyclePolicy.ts#L180">property <b>selection</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>selection: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='s2'>"untagged"</span> | <span class='s2'>"any"</span> | {
    tagPrefixList: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
}&gt;;</pre>
{{% md %}}

Determines whether the lifecycle policy rule that you are adding specifies a tag for an
image. If you specify `any`, then all images have the rule applied to them. If you specify
`untagged` then the rule will only apply to untagged images.  Otherwise, you can specify a
`tagPrefixList` value.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="RepositoryArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L75">interface <b>RepositoryArgs</b></a>
</h2>
<div class="pdoc-module-contents">
<h3 class="pdoc-member-header" id="RepositoryArgs-lifeCyclePolicyArgs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L90">property <b>lifeCyclePolicyArgs</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>lifeCyclePolicyArgs?: <a href='#LifecyclePolicyArgs'>LifecyclePolicyArgs</a>;</pre>
{{% md %}}

The arguments controlling the [LifecyclePolicy] for this [Repository].  If `undefined`, a default one will be
created using `LifecyclePolicy.getDefaultLifecyclePolicyArgs`.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="RepositoryArgs-repository">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L79">property <b>repository</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>repository?: aws.ecr.Repository;</pre>
{{% md %}}

Underlying repository.  If not provided, a new one will be created on your behalf.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="RepositoryArgs-tags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-awsx/blob/4efcf0b7e124489da16fc08702b4fe5c9837ea2c/nodejs/awsx/ecr/repository.ts#L84">property <b>tags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>tags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;Record&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>&gt;&gt;;</pre>
{{% md %}}

A mapping of tags to assign to the resource.

{{% /md %}}
</div>
</div>
