<script>
  import Basics from "./lib/01. introduction/a_Basics.svelte";
  import AddingData from "./lib/01. introduction/b_AddingData.svelte";
  import DynamicAttributes from "./lib/01. introduction/c_DynamicAttributes.svelte";
  import Styling from "./lib/01. introduction/d_Styling.svelte";
  import NestedComponents from "./lib/01. introduction/e_NestedComponents.svelte";
  import HtmlTags from "./lib/01. introduction/f_HtmlTags.svelte";
  import Assignments from "./lib/02. reactivity/a_Assignments.svelte";
  import Declarations from "./lib/02. reactivity/b_Declarations.svelte";
  import Statements from "./lib/02. reactivity/c_Statements.svelte";
  import UpdatingArrayAndObject from "./lib/02. reactivity/d_UpdatingArrayAndObject.svelte";
  import DeclaringProps from "./lib/03. Props/a_DeclaringProps.svelte";
  import DefaultValues from "./lib/03. Props/b_DefaultValues.svelte";
  import SpreadProps from "./lib/03. Props/c_SpreadProps.svelte";
  import IfBlocks from "./lib/04. Logic/a_IfBlocks.svelte";
  import ElseBlocks from "./lib/04. Logic/b_ElseBlocks.svelte";
  import ElseIfBlocks from "./lib/04. Logic/c_ElseIfBlocks.svelte";
  import EachBlocks from "./lib/04. Logic/d_EachBlocks.svelte";
  import KeyedEachBlocks from "./lib/04. Logic/e_KeyedEachBlocks.svelte";
  import AwaitBlocks from "./lib/04. Logic/f_AwaitBlocks.svelte";
  import DOMEvents from "./lib/05. Events/a_DOMEvents.svelte";
  import InlineHandlers from "./lib/05. Events/b_InlineHandlers.svelte";
  import EventModifiers from "./lib/05. Events/c_EventModifiers.svelte";
  import ComponentEvents from "./lib/05. Events/d_ComponentEvents.svelte";
  import EventForwarding from "./lib/05. Events/e_EventForwarding.svelte";
  import DOMEventForwarding from "./lib/05. Events/f_DOMEventForwarding.svelte";
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
  <!-- 04. Logic -->
  <IfBlocks />
  <ElseBlocks />
  <ElseIfBlocks />
  <EachBlocks />
  <KeyedEachBlocks />
  <AwaitBlocks />
  <!-- 05. Events -->
  <DOMEvents />
  <InlineHandlers />
  <EventModifiers />
  <ComponentEvents on:message={(e) => alert(e.detail.text)} />
  <EventForwarding on:message={(e) => alert(e.detail.text)} />
  <DOMEventForwarding on:click={() => alert("click")} />
</main>

<style>
</style>
