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

  import TextInputs from "./lib/06. Bindings/a_TextInputs.svelte";
  import NumericInputs from "./lib/06. Bindings/b_NumericInputs.svelte";
  import CheckboxInputs from "./lib/06. Bindings/c_CheckboxInputs.svelte";
  import GroupInputs from "./lib/06. Bindings/d_GroupInputs.svelte";
  import TextareaInputs from "./lib/06. Bindings/e_TextareaInputs.svelte";
  import SelectBindings from "./lib/06. Bindings/f_SelectBindings.svelte";
  import SelectMultiple from "./lib/06. Bindings/g_SelectMultiple.svelte";
  import ContenteditableBindings from "./lib/06. Bindings/h_ContenteditableBindings.svelte";
  import EachBlockBindings from "./lib/06. Bindings/i_EachBlockBindings.svelte";
  import MediaElements from "./lib/06. Bindings/j_MediaElements.svelte";
  import Dimensions from "./lib/06. Bindings/k_Dimensions.svelte";
  import This from "./lib/06. Bindings/l_This.svelte";
  import ComponentBindings from "./lib/06. Bindings/m_ComponentBindings.svelte";
  import BindingToComponentInstances from "./lib/06. Bindings/n_BindingToComponentInstances.svelte";

  import OnMount from "./lib/07. Lifecycle/a_OnMount.svelte";
  import OnDestroy from "./lib/07. Lifecycle/b_OnDestroy.svelte";
  import BeforeUpdate from "./lib/07. Lifecycle/c_BeforeUpdate.svelte";
  import Tick from "./lib/07. Lifecycle/d_Tick.svelte";

  import WritableStores from "./lib/08. Stores/a_WritableStores/App.svelte";
  import AutoSubscriptions from "./lib/08. Stores/b_AutoSubscriptions/App.svelte";
  import ReadableStores from "./lib/08. Stores/c_ReadableStores/App.svelte";
  import DerivedStores from "./lib/08. Stores/d_DerivedStores/App.svelte";
  import CustomStores from "./lib/08. Stores/e_CustomStores/App.svelte";
  import StoreBindings from "./lib/08. Stores/f_StoreBindings/App.svelte";

  import Tweened from "./lib/09. Motion/a_Tweened.svelte";
  import Spring from "./lib/09. Motion/b_Spring.svelte";

  import TheTransitionDirective from "./lib/10. Transitions/a_TheTransitionDirective.svelte";
  import AddingParameters from "./lib/10. Transitions/b_AddingParameters.svelte";
  import InAndOut from "./lib/10. Transitions/c_InAndOut.svelte";
  import CustomCssTransitions from "./lib/10. Transitions/d_CustomCssTransitions.svelte";
  import TransitionEvents from "./lib/10. Transitions/e_TransitionEvents.svelte";
  import LocalTransitions from "./lib/10. Transitions/f_LocalTransitions.svelte";
  import DeferredTransitions from "./lib/10. Transitions/g_DeferredTransitions.svelte";
  import KeyBlocks from "./lib/10. Transitions/h_KeyBlocks.svelte";

  import TheAnimateDirective from "./lib/11. Animations/a_TheAnimateDirective.svelte";

  import TheUseDirective from "./lib/12. Actions/a_TheUseDirective.svelte";
  import ActionAddingParameters from "./lib/12. Actions/b_AddingParameters.svelte";

  import TheClassDirective from "./lib/13. Advanced Styling/a_TheClassDirective.svelte";
  import ShorthandClassDirective from "./lib/13. Advanced Styling/b_ShorthandClassDirective.svelte";
  import InlineStyles from "./lib/13. Advanced Styling/c_InlineStyles.svelte";
  import TheStyleDirective from "./lib/13. Advanced Styling/d_TheStyleDirective.svelte";

  import Slots from "./lib/14. Component composition/a. Slots/a_Slots.svelte";
  import SlotFallback from "./lib/14. Component composition/b. Slot fallback/b_SlotFallback.svelte";
  import NamedSlots from "./lib/14. Component composition/c. Named slots/c_NamedSlots.svelte";
  import CheckingForSlotContent from "./lib/14. Component composition/d. Checking for slot content/d_CheckingForSlotContent.svelte";
  import SlotProps from "./lib/14. Component composition/e. Slot props/e_SlotProps.svelte";

  import SetContextAndGetContext from "./lib/15. Context API/a_SetContextAndGetContext.svelte";
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

  <!-- 06. Bindings -->
  <TextInputs />
  <NumericInputs />
  <CheckboxInputs />
  <GroupInputs />
  <TextareaInputs />
  <SelectBindings />
  <SelectMultiple />
  <ContenteditableBindings />
  <EachBlockBindings />
  <MediaElements />
  <Dimensions />
  <This />
  <ComponentBindings />
  <BindingToComponentInstances />

  <!-- 07. LifeCycle -->
  <OnMount />
  <OnDestroy />
  <BeforeUpdate />
  <Tick />

  <!-- 08. Stores -->
  <WritableStores />
  <AutoSubscriptions />
  <ReadableStores />
  <DerivedStores />
  <CustomStores />
  <StoreBindings />

  <!-- 09. Motion -->
  <Tweened />
  <Spring />

  <!-- 10. Transitions -->
  <TheTransitionDirective />
  <AddingParameters />
  <InAndOut />
  <CustomCssTransitions />
  <TransitionEvents />
  <LocalTransitions />
  <DeferredTransitions />
  <KeyBlocks />

  <!-- 11. Animations -->
  <TheAnimateDirective />

  <!-- 12. Actions -->
  <TheUseDirective />
  <ActionAddingParameters />

  <!-- 13. Advanced Styling -->
  <TheClassDirective />
  <ShorthandClassDirective />
  <InlineStyles />
  <TheStyleDirective />

  <!-- 14. Component composition -->
  <Slots />
  <SlotFallback />
  <NamedSlots />
  <CheckingForSlotContent />
  <SlotProps />

  <!-- 15. Context API -->
  <SetContextAndGetContext />
</main>

<style>
</style>
