<script>
  import Navbar from '$lib/components/Navbar.svelte';
  import Hero from '$lib/components/Hero.svelte';
  import ProblemSection from '$lib/components/ProblemSection.svelte';
  import SpeedSection from '$lib/components/SpeedSection.svelte';
  import PlatformFeatures from '$lib/components/PlatformFeatures.svelte';
  import ROISection from '$lib/components/ROISection.svelte';
  import EnterpriseTrust from '$lib/components/EnterpriseTrust.svelte';
  import FooterSection from '$lib/components/FooterSection.svelte';
</script>

<main class="font-sans antialiased text-gray-900 bg-white selection:bg-gray-100 selection:text-gray-900">
  <Navbar />
  <Hero />
  <ProblemSection />
  <SpeedSection />
  <PlatformFeatures />
  <ROISection />
  <EnterpriseTrust />
  <FooterSection />
</main>

