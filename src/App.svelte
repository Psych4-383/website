<script>
    import Nav from './components/Nav.svelte';
    import {Router, Route, navigate} from 'svelte-navigator';
    import LandingPage from './pages/LandingPage.svelte';
    import AboutPage from './pages/AboutPage.svelte';
    import MemberPage from './pages/MemberPage.svelte';
    import EventPage from './pages/EventPage.svelte';
    import LearnPage from './pages/LearnPage.svelte';
    import Robopage from './pages/RoboPage.svelte';
    import MobileNav from './components/MobileNav.svelte';
    import RoboEventPage from './pages/RoboEventPage.svelte';
    import TGPage from './pages/TGPage.svelte';
</script>
<Router>
    <MobileNav />
    <Nav />
    <Route path="learn" component={LearnPage}/>
    <Route path="about" component={AboutPage}/>
    <Route path="tg" component={TGPage}/>
    <Route path="team" component={MemberPage}/>
    <Route path="event" component={EventPage}/>
    <Route path="robo" component={Robopage}/>
    <Route path="/" component={LandingPage} />
    <Route path="/roboEvent" component={RoboEventPage} />
</Router>
