<script>
  import ABasics from "./lib/01. introduction/a_Basics.svelte";
  import Basics from "./lib/01. introduction/a_Basics.svelte";
  import AddingData from "./lib/01. introduction/b_AddingData.svelte";
  import DynamicAttributes from "./lib/01. introduction/c_DynamicAttributes.svelte";
  import Styling from "./lib/01. introduction/d_Styling.svelte";
  import NestedComponents from "./lib/01. introduction/e_NestedComponents.svelte";
  import HtmlTags from "./lib/01. introduction/f_HtmlTags.svelte";
  import AAssignments from "./lib/02. reactivity/a_Assignments.svelte";
  import Assignments from "./lib/02. reactivity/a_Assignments.svelte";
  import Declarations from "./lib/02. reactivity/b_Declarations.svelte";
  import Statements from "./lib/02. reactivity/c_Statements.svelte";
  import UpdatingArrayAndObject from "./lib/02. reactivity/d_UpdatingArrayAndObject.svelte";
  import DeclaringProps from "./lib/03. Props/a_DeclaringProps.svelte";
  import DefaultValues from "./lib/03. Props/b_DefaultValues.svelte";
  import SpreadProps from "./lib/03. Props/c_SpreadProps.svelte";
</script>

<main>
  <!-- 01. introduction -->
  <Basics />
  <AddingData />
  <DynamicAttributes />
  <Styling />
  <NestedComponents />
  <HtmlTags />
  <!-- 02. reactivity -->
  <Assignments />
  <Declarations />
  <Statements />
  <UpdatingArrayAndObject />
  <!-- 03. Props -->
  <DeclaringProps answer={30} />
  <DefaultValues />
  <SpreadProps {...{ name: "doe", age: 30 }} />
</main>

<style>
</style>
