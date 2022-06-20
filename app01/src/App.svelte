<script>
import IfElse from './components/conditional-comp/if-else.svelte';

  import logo from './assets/svelte.png'
  import Counter from './lib/Counter.svelte'
  import Helloworld from './components/helloworld/Helloworld.svelte';
  import WorkingWithSvelte from './components/working-with-svelte/working-with-svelte.svelte';
  import Photo from './components/img/Img.svelte';
 import CssSvelte from './components/css-svelte/css-svelte.svelte';
 import Timer from './components/timer/timer.svelte';
 import Square from './components/square-number/square.svelte';
 import AddEven from './components/add-even-number/add-even.svelte';
 import PropsEx from './components/props-example/props-ex.svelte';
import EmotionCss from './components/emotion-css/emotion-css.svelte';
import Img from './components/img/Img.svelte';
import ConditionalComp from './components/conditional-comp/conditional-comp.svelte';
import NestedConditional from './components/conditional-comp/nested-conditional.svelte';
import Ifelse from './components/conditional-comp/if-else.svelte';
import LoopHtml from './components/movie-loop-html/movie-loop-html.svelte';
const status = false;
 const user01 = {
        imageUrl :'https://i.pravatar.cc/200?u=a042581f4e290267044',
        name:'Rajesh Singh',		
        role:'Photographer'
  }
  </script>

<!-- <Helloworld />
<WorkingWithSvelte />
<Photo />
<Timer />
<Square /> -->
<!-- <CssSvelte /> -->
<!-- <AddEven />
<PropsEx 
{...user01}
/>
<ConditionalComp {status} />
<NestedConditional />
<Ifelse /> -->
<LoopHtml />
<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  img {
    height: 16rem;
    width: 16rem;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4rem;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  p {
    max-width: 14rem;
    margin: 1rem auto;
    line-height: 1.35;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
