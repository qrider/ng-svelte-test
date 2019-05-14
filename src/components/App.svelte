<script>
  import { Router, Route, Link } from 'svero';

  import Test1 from './Test1.svelte';
  import Test2 from './Test2.svelte';
  import Index from './Index.svelte';
</script>

<Router>
  <Route path="*" component={Index} />
  <Route path="/test1" component={Test1} />
  <Route path="/test2" component={Test2} />
</Router>


<ul>
  <li>
    <Link href="/test1" className="btn">Test1</Link>
  </li>
  <li>
    <Link href="/test2" className="btn">Test2</Link>
  </li>
</ul>


