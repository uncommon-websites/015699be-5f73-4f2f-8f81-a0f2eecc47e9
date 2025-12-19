<script>
  let activeTab = 'Workflow';
  const tabs = ['Workflow', 'Integration', 'Analytics', 'Security'];
</script>

<section class="py-24 bg-gray-50 text-center">
  <div class="max-w-[1200px] mx-auto px-6">
    <h2 class="text-5xl font-bold mb-6 tracking-tight text-gray-900">
      Enterprise-Grade<br>Platform Capabilities
    </h2>
    
    <!-- Tabs -->
    <div class="flex justify-center mb-8">
      <div class="bg-white p-1 rounded-lg inline-flex shadow-sm border border-gray-200">
        {#each tabs as tab}
          <button 
            class="px-4 py-1.5 text-sm font-medium rounded-md transition-all {activeTab === tab ? 'bg-gray-900 text-white shadow-sm' : 'text-gray-500 hover:text-gray-700'}"
            on:click={() => activeTab = tab}
          >
            {tab}
          </button>
        {/each}
      </div>
    </div>

    <p class="text-lg text-gray-600 mb-16 max-w-2xl mx-auto leading-relaxed">
      Everything you need to build, deploy, and manage enterprise software solutions that scale with your business.
    </p>

    <!-- Feature Showcase -->
    <div class="bg-white rounded-xl shadow-xl overflow-hidden border border-gray-200 text-left max-w-5xl mx-auto">
      {#if activeTab === 'Workflow'}
        <div class="p-12">
          <div class="grid grid-cols-2 gap-12">
            <div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Streamlined Workflows</h3>
              <p class="text-gray-600 mb-6 leading-relaxed">
                Automate complex business processes with intuitive workflow builders. No coding required for common scenarios.
              </p>
              <ul class="space-y-3 text-sm text-gray-700">
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Visual workflow designer</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Automated approvals and routing</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Real-time notifications</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Custom business rules</span>
                </li>
              </ul>
            </div>
            <div class="bg-gradient-to-br from-gray-100 to-gray-200 rounded-lg p-8 flex items-center justify-center">
              <div class="text-center">
                <div class="text-6xl mb-4">⚡</div>
                <div class="text-sm font-semibold text-gray-700">Workflow Automation</div>
              </div>
            </div>
          </div>
        </div>
      {:else if activeTab === 'Integration'}
        <div class="p-12">
          <div class="grid grid-cols-2 gap-12">
            <div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Seamless Integration</h3>
              <p class="text-gray-600 mb-6 leading-relaxed">
                Connect with your existing enterprise systems through pre-built integrations and powerful APIs.
              </p>
              <ul class="space-y-3 text-sm text-gray-700">
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>RESTful API access</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>SSO and identity management</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Database connectivity</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Third-party service integration</span>
                </li>
              </ul>
            </div>
            <div class="bg-gradient-to-br from-gray-100 to-gray-200 rounded-lg p-8 flex items-center justify-center">
              <div class="text-center">
                <div class="text-6xl mb-4">🔗</div>
                <div class="text-sm font-semibold text-gray-700">Enterprise Integration</div>
              </div>
            </div>
          </div>
        </div>
      {:else if activeTab === 'Analytics'}
        <div class="p-12">
          <div class="grid grid-cols-2 gap-12">
            <div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Powerful Analytics</h3>
              <p class="text-gray-600 mb-6 leading-relaxed">
                Make data-driven decisions with comprehensive analytics and customizable reporting dashboards.
              </p>
              <ul class="space-y-3 text-sm text-gray-700">
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Real-time dashboards</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Custom report builder</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Data visualization tools</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Automated insights</span>
                </li>
              </ul>
            </div>
            <div class="bg-gradient-to-br from-gray-100 to-gray-200 rounded-lg p-8 flex items-center justify-center">
              <div class="text-center">
                <div class="text-6xl mb-4">📊</div>
                <div class="text-sm font-semibold text-gray-700">Business Intelligence</div>
              </div>
            </div>
          </div>
        </div>
      {:else if activeTab === 'Security'}
        <div class="p-12">
          <div class="grid grid-cols-2 gap-12">
            <div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Enterprise Security</h3>
              <p class="text-gray-600 mb-6 leading-relaxed">
                Bank-level security and compliance built into every layer of your custom software solution.
              </p>
              <ul class="space-y-3 text-sm text-gray-700">
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>End-to-end encryption</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Role-based access control</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Compliance certifications</span>
                </li>
                <li class="flex items-start gap-2">
                  <span class="text-green-600 mt-0.5">✓</span>
                  <span>Audit logging and monitoring</span>
                </li>
              </ul>
            </div>
            <div class="bg-gradient-to-br from-gray-100 to-gray-200 rounded-lg p-8 flex items-center justify-center">
              <div class="text-center">
                <div class="text-6xl mb-4">🔒</div>
                <div class="text-sm font-semibold text-gray-700">Security & Compliance</div>
              </div>
            </div>
          </div>
        </div>
      {/if}
    </div>
  </div>
</section>
