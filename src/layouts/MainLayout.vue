<template>
  v<template>
    <div class="min-h-screen bg-gradient-to-br from-violet-500/20 via-white to-rose-200/10 p-4">
      <div
        class="max-w-[1200px] mx-auto bg-transparent rounded-2xl overflow-hidden border border-gray-300 shadow-2xl"
      >
        <div class="flex">
          <!-- SIDEBAR -->
          <aside
            class="w-36 p-3 border-r border-gray-200 h-screen bg-gradient-to-b from-white/30 to-white/10"
          >
            <div class="text-center mt-2">
              <div
                class="w-12 h-12 mx-auto rounded-lg bg-gradient-to-br from-teal-600 to-cyan-500 text-white flex items-center justify-center font-bold"
              >
                TR
              </div>
              <h2 class="mt-2 font-bold text-lg">Trinita</h2>
            </div>
            <ul class="mt-6 space-y-2 text-sm">
              <li class="sidebar-item px-2 py-1 rounded-lg bg-teal-800 text-white">Dashboard</li>
              <li class="sidebar-item px-2 py-1 rounded-lg">Squad</li>
              <li class="sidebar-item px-2 py-1 rounded-lg">Messager</li>
              <li class="sidebar-item px-2 py-1 rounded-lg">Statistic</li>
              <li class="sidebar-item px-2 py-1 rounded-lg">Calendar</li>
              <li class="sidebar-item px-2 py-1 rounded-lg">Finance</li>
            </ul>
          </aside>

          <!-- CONTENT -->
          <div class="flex-1 flex flex-col">
            <!-- HEADER -->
            <header
              class="flex items-center justify-between p-4 border-b border-gray-200 bg-white/40"
            >
              <div class="text-sm text-teal-700 font-semibold">Welcome Back, Triwahyuni</div>
              <div class="flex items-center gap-4">
                <!-- search -->
                <div class="relative">
                  <input
                    type="text"
                    placeholder="Search..."
                    class="rounded-lg pl-8 pr-3 py-1 text-sm border border-gray-300 focus:outline-none focus:ring-1 focus:ring-teal-400"
                  />
                  <span class="absolute left-2 top-1.5 text-sm text-gray-500">🔍</span>
                </div>
                <!-- icons -->
                <button
                  title="Notifications"
                  class="w-8 h-8 rounded-full bg-amber-400 flex items-center justify-center"
                >
                  🔔
                </button>
                <button
                  title="Messages"
                  class="w-8 h-8 rounded-full bg-sky-400 flex items-center justify-center"
                >
                  💬
                </button>
                <div class="flex items-center gap-2">
                  <div
                    class="w-8 h-8 rounded-full bg-gradient-to-br from-amber-600 to-yellow-400 flex items-center justify-center text-white font-bold"
                  >
                    TA
                  </div>
                  <div class="font-semibold">Triwahyuni</div>
                </div>
              </div>
            </header>

            <!-- MAIN GRID -->
            <main class="p-6 overflow-y-auto">
              <h1 class="text-3xl font-semibold mb-4">Dashboard</h1>

              <div class="grid grid-cols-3 gap-6">
                <!-- LEFT: Next Game + Standings (stack) -->
                <div class="col-span-2 flex flex-col gap-6">
                  <!-- NEXT GAME -->
                  <div class="card">
                    <div class="flex justify-between items-center mb-3">
                      <h3 class="text-lg font-bold">Next game</h3>
                      <a href="#" class="text-sm text-teal-600 font-semibold">View calendar</a>
                    </div>

                    <div class="flex items-center justify-center gap-8 mt-2">
                      <div class="flex flex-col items-center">
                        <img
                          src="https://upload.wikimedia.org/wikipedia/commons/1/15/Juventus_FC_2017_logo.svg"
                          alt="juventus"
                          class="w-12 h-12"
                        />
                        <span class="mt-2 font-semibold">Juventus</span>
                      </div>

                      <div class="text-2xl font-extrabold text-gray-700">VS</div>

                      <div class="flex flex-col items-center">
                        <img
                          src="https://upload.wikimedia.org/wikipedia/en/5/5b/US_Sassuolo_Calcio_logo.svg"
                          alt="sassuolo"
                          class="w-12 h-12"
                        />
                        <span class="mt-2 font-semibold">Sassuolo</span>
                      </div>
                    </div>

                    <p class="text-center text-sm text-gray-600 mt-4">
                      Serie A | 21:00, 11 November 2020
                    </p>
                  </div>

                  <!-- STANDINGS -->
                  <div class="card">
                    <div class="flex justify-between items-center mb-3">
                      <h3 class="text-lg font-bold">Standings</h3>
                      <a href="#" class="text-sm text-teal-600 font-semibold">View all</a>
                    </div>

                    <div class="overflow-x-auto">
                      <table class="w-full text-sm text-gray-700">
                        <thead class="text-xs text-gray-600 border-b border-gray-300">
                          <tr>
                            <th class="py-2 text-left">#</th>
                            <th class="py-2 text-left">Team</th>
                            <th class="py-2 text-center">P</th>
                            <th class="py-2 text-center">W</th>
                            <th class="py-2 text-center">D</th>
                            <th class="py-2 text-center">L</th>
                            <th class="py-2 text-center">Pts</th>
                          </tr>
                        </thead>
                        <tbody>
                          <tr class="border-b border-gray-200 hover:bg-white/60">
                            <td class="py-2">1</td>
                            <td class="py-2 flex items-center gap-3">
                              <img
                                src="https://upload.wikimedia.org/wikipedia/commons/1/15/Juventus_FC_2017_logo.svg"
                                class="w-6 h-6"
                                alt="Juventus"
                              />
                              <span>Juventus</span>
                            </td>
                            <td class="text-center">8</td>
                            <td class="text-center">6</td>
                            <td class="text-center">1</td>
                            <td class="text-center">1</td>
                            <td class="text-center font-bold text-teal-700">19</td>
                          </tr>

                          <tr class="border-b border-gray-200 hover:bg-white/60">
                            <td class="py-2">2</td>
                            <td class="py-2 flex items-center gap-3">
                              <img
                                src="https://upload.wikimedia.org/wikipedia/en/0/0c/AS_Roma_logo_%282017%29.svg"
                                class="w-6 h-6"
                                alt="AS Roma"
                              />
                              <span>AS Roma</span>
                            </td>
                            <td class="text-center">8</td>
                            <td class="text-center">5</td>
                            <td class="text-center">1</td>
                            <td class="text-center">2</td>
                            <td class="text-center font-bold">16</td>
                          </tr>

                          <tr class="border-b border-gray-200 hover:bg-white/60">
                            <td class="py-2">3</td>
                            <td class="py-2 flex items-center gap-3">
                              <img
                                src="https://upload.wikimedia.org/wikipedia/en/0/05/SSC_Napoli_logo_2021.svg"
                                class="w-6 h-6"
                                alt="Napoli"
                              />
                              <span>Napoli</span>
                            </td>
                            <td class="text-center">8</td>
                            <td class="text-center">5</td>
                            <td class="text-center">0</td>
                            <td class="text-center">3</td>
                            <td class="text-center font-bold">15</td>
                          </tr>

                          <tr class="border-b border-gray-200 hover:bg-white/60">
                            <td class="py-2">4</td>
                            <td class="py-2 flex items-center gap-3">
                              <img
                                src="https://upload.wikimedia.org/wikipedia/en/e/e1/Inter_Milan_2021_logo.svg"
                                class="w-6 h-6"
                                alt="Inter"
                              />
                              <span>Inter</span>
                            </td>
                            <td class="text-center">8</td>
                            <td class="text-center">4</td>
                            <td class="text-center">1</td>
                            <td class="text-center">3</td>
                            <td class="text-center font-bold">13</td>
                          </tr>

                          <tr class="hover:bg-white/60">
                            <td class="py-2">5</td>
                            <td class="py-2 flex items-center gap-3">
                              <img
                                src="https://upload.wikimedia.org/wikipedia/en/5/5b/US_Sassuolo_Calcio_logo.svg"
                                class="w-6 h-6"
                                alt="Sassuolo"
                              />
                              <span>Sassuolo</span>
                            </td>
                            <td class="text-center">8</td>
                            <td class="text-center">4</td>
                            <td class="text-center">1</td>
                            <td class="text-center">3</td>
                            <td class="text-center font-bold">13</td>
                          </tr>
                        </tbody>
                      </table>
                    </div>
                  </div>
                </div>

                <!-- RIGHT: Stats, Game Statistic, Reminder -->
                <div class="flex flex-col gap-6">
                  <!-- Game Statistic -->
                  <div class="card">
                    <div class="flex justify-between items-center mb-3">
                      <h3 class="text-lg font-bold">Games statistic</h3>
                      <a href="#" class="text-sm text-teal-600 font-semibold">View all statistic</a>
                    </div>

                    <!-- segmented bar matching image: victories (teal), draws (gray), lost (pink) -->
                    <div class="seg-wrap w-full rounded-full mt-2" aria-hidden>
                      <!-- Victories 75% -->
                      <div
                        class="seg"
                        style="
                          left: 0;
                          width: 75%;
                          background: linear-gradient(90deg, #0ea5a4, #06b6d4);
                        "
                      ></div>
                      <!-- Draws 10% -->
                      <div
                        class="seg"
                        style="
                          left: 75%;
                          width: 10%;
                          background: linear-gradient(90deg, #d1d5db, #9ca3af);
                        "
                      ></div>
                      <!-- Lost 15% -->
                      <div
                        class="seg"
                        style="
                          left: 85%;
                          width: 15%;
                          background: linear-gradient(90deg, #f9a8d4, #f472b6);
                        "
                      ></div>
                    </div>

                    <div class="flex justify-between mt-3 text-sm text-gray-700 font-medium">
                      <span>PL 8</span>
                      <span>Victories 6</span>
                      <span>Draws 1</span>
                      <span>Lost 1</span>
                    </div>
                  </div>

                  <!-- Small Stats grid -->
                  <div class="grid grid-cols-2 gap-3">
                    <div class="card p-3 text-center">
                      <div class="text-xs text-gray-500">Possession</div>
                      <div class="text-2xl font-bold">65%</div>
                      <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                        <div class="h-2 rounded-full" style="width: 65%; background: #10b981"></div>
                      </div>
                    </div>

                    <div class="card p-3 text-center">
                      <div class="text-xs text-gray-500">Overall price</div>
                      <div class="text-2xl font-bold">$690.2m</div>
                      <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                        <div
                          class="h-2 rounded-full"
                          style="width: 100%; background: #14b8a6"
                        ></div>
                      </div>
                    </div>

                    <div class="card p-3 text-center">
                      <div class="text-xs text-gray-500">Transfer budget</div>
                      <div class="text-2xl font-bold">$240.6m</div>
                      <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                        <div class="h-2 rounded-full" style="width: 75%; background: #fb923c"></div>
                      </div>
                    </div>

                    <div class="card p-3 text-center">
                      <div class="text-xs text-gray-500">Average score</div>
                      <div class="text-2xl font-bold">7.2</div>
                      <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                        <div class="h-2 rounded-full" style="width: 72%; background: #60a5fa"></div>
                      </div>
                    </div>
                  </div>

                  <!-- Reminder -->
                  <div
                    class="rounded-xl p-4 shadow-xl bg-gradient-to-r from-teal-600 to-green-400 text-white flex items-center justify-between"
                  >
                    <div>
                      <div class="font-bold text-lg">Don't forget</div>
                      <div class="font-semibold text-sm mt-1">Setup training for next week</div>
                      <div class="text-xs mt-1">
                        Go to training center to plan tactical drills and recovery session
                      </div>
                    </div>
                    <div class="flex flex-col items-center gap-3">
                      <div
                        class="w-16 h-16 rounded-lg bg-white/20 flex items-center justify-center text-2xl"
                      >
                        🎯
                      </div>
                      <button
                        class="bg-white text-teal-700 px-3 py-1 rounded-lg font-semibold text-sm"
                      >
                        Go to training center
                      </button>
                    </div>
                  </div>
                </div>
              </div>

              <!-- FOOTER -->
              <div class="mt-6 text-center text-xs text-gray-600">
                © 2025 Trinita Dashboard — Triwahyuni Vanisa Akili
              </div>
            </main>
          </div>
        </div>
      </div>
    </div>
  </template>
  <script setup></script>

  <div class="min-h-screen bg-gradient-to-br from-violet-500/20 via-white to-rose-200/10 p-4">
    <div
      class="max-w-[1200px] mx-auto bg-transparent rounded-2xl overflow-hidden border border-gray-300 shadow-2xl"
    >
      <div class="flex">
        <!-- SIDEBAR -->

        <aside
          class="w-36 p-3 border-r border-gray-200 h-screen bg-gradient-to-b from-white/30 to-white/10"
        >
          <div class="text-center mt-2">
            <div
              class="w-12 h-12 mx-auto rounded-lg bg-gradient-to-br from-teal-600 to-cyan-500 text-white flex items-center justify-center font-bold"
            >
              TR
            </div>

            <h2 class="mt-2 font-bold text-lg">Trinita</h2>
          </div>

          <ul class="mt-6 space-y-2 text-sm">
            <li class="sidebar-item px-2 py-1 rounded-lg bg-teal-800 text-white">Dashboard</li>

            <li class="sidebar-item px-2 py-1 rounded-lg">Squad</li>

            <li class="sidebar-item px-2 py-1 rounded-lg">Messager</li>

            <li class="sidebar-item px-2 py-1 rounded-lg">Statistic</li>

            <li class="sidebar-item px-2 py-1 rounded-lg">Calendar</li>

            <li class="sidebar-item px-2 py-1 rounded-lg">Finance</li>
          </ul>
        </aside>

        <!-- CONTENT -->

        <div class="flex-1 flex flex-col">
          <!-- HEADER -->

          <header
            class="flex items-center justify-between p-4 border-b border-gray-200 bg-white/40"
          >
            <div class="text-sm text-teal-700 font-semibold">Welcome Back, Triwahyuni</div>

            <div class="flex items-center gap-4">
              <!-- search -->

              <div class="relative">
                <input
                  type="text"
                  placeholder="Search..."
                  class="rounded-lg pl-8 pr-3 py-1 text-sm border border-gray-300 focus:outline-none focus:ring-1 focus:ring-teal-400"
                />

                <span class="absolute left-2 top-1.5 text-sm text-gray-500">🔍</span>
              </div>

              <!-- icons -->

              <button
                title="Notifications"
                class="w-8 h-8 rounded-full bg-amber-400 flex items-center justify-center"
              >
                🔔
              </button>

              <button
                title="Messages"
                class="w-8 h-8 rounded-full bg-sky-400 flex items-center justify-center"
              >
                💬
              </button>

              <div class="flex items-center gap-2">
                <div
                  class="w-8 h-8 rounded-full bg-gradient-to-br from-amber-600 to-yellow-400 flex items-center justify-center text-white font-bold"
                >
                  TA
                </div>

                <div class="font-semibold">Triwahyuni</div>
              </div>
            </div>
          </header>

          <!-- MAIN GRID -->

          <main class="p-6 overflow-y-auto">
            <h1 class="text-3xl font-semibold mb-4">Dashboard</h1>

            <div class="grid grid-cols-3 gap-6">
              <!-- LEFT: Next Game + Standings (stack) -->

              <div class="col-span-2 flex flex-col gap-6">
                <!-- NEXT GAME -->

                <div class="card">
                  <div class="flex justify-between items-center mb-3">
                    <h3 class="text-lg font-bold">Next game</h3>

                    <a href="#" class="text-sm text-teal-600 font-semibold">View calendar</a>
                  </div>

                  <div class="flex items-center justify-center gap-8 mt-2">
                    <div class="flex flex-col items-center">
                      <img
                        src="https://upload.wikimedia.org/wikipedia/commons/1/15/Juventus_FC_2017_logo.svg"
                        alt="juventus"
                        class="w-12 h-12"
                      />

                      <span class="mt-2 font-semibold">Juventus</span>
                    </div>

                    <div class="text-2xl font-extrabold text-gray-700">VS</div>

                    <div class="flex flex-col items-center">
                      <img
                        src="https://upload.wikimedia.org/wikipedia/en/5/5b/US_Sassuolo_Calcio_logo.svg"
                        alt="sassuolo"
                        class="w-12 h-12"
                      />

                      <span class="mt-2 font-semibold">Sassuolo</span>
                    </div>
                  </div>

                  <p class="text-center text-sm text-gray-600 mt-4">
                    Serie A | 21:00, 11 November 2020
                  </p>
                </div>

                <!-- STANDINGS -->

                <div class="card">
                  <div class="flex justify-between items-center mb-3">
                    <h3 class="text-lg font-bold">Standings</h3>

                    <a href="#" class="text-sm text-teal-600 font-semibold">View all</a>
                  </div>

                  <div class="overflow-x-auto">
                    <table class="w-full text-sm text-gray-700">
                      <thead class="text-xs text-gray-600 border-b border-gray-300">
                        <tr>
                          <th class="py-2 text-left">#</th>

                          <th class="py-2 text-left">Team</th>

                          <th class="py-2 text-center">P</th>

                          <th class="py-2 text-center">W</th>

                          <th class="py-2 text-center">D</th>

                          <th class="py-2 text-center">L</th>

                          <th class="py-2 text-center">Pts</th>
                        </tr>
                      </thead>

                      <tbody>
                        <tr class="border-b border-gray-200 hover:bg-white/60">
                          <td class="py-2">1</td>

                          <td class="py-2 flex items-center gap-3">
                            <img
                              src="https://upload.wikimedia.org/wikipedia/commons/1/15/Juventus_FC_2017_logo.svg"
                              class="w-6 h-6"
                              alt="Juventus"
                            />

                            <span>Juventus</span>
                          </td>

                          <td class="text-center">8</td>

                          <td class="text-center">6</td>

                          <td class="text-center">1</td>

                          <td class="text-center">1</td>

                          <td class="text-center font-bold text-teal-700">19</td>
                        </tr>

                        <tr class="border-b border-gray-200 hover:bg-white/60">
                          <td class="py-2">2</td>

                          <td class="py-2 flex items-center gap-3">
                            <img
                              src="https://upload.wikimedia.org/wikipedia/en/0/0c/AS_Roma_logo_%282017%29.svg"
                              class="w-6 h-6"
                              alt="AS Roma"
                            />

                            <span>AS Roma</span>
                          </td>

                          <td class="text-center">8</td>

                          <td class="text-center">5</td>

                          <td class="text-center">1</td>

                          <td class="text-center">2</td>

                          <td class="text-center font-bold">16</td>
                        </tr>

                        <tr class="border-b border-gray-200 hover:bg-white/60">
                          <td class="py-2">3</td>

                          <td class="py-2 flex items-center gap-3">
                            <img
                              src="https://upload.wikimedia.org/wikipedia/en/0/05/SSC_Napoli_logo_2021.svg"
                              class="w-6 h-6"
                              alt="Napoli"
                            />

                            <span>Napoli</span>
                          </td>

                          <td class="text-center">8</td>

                          <td class="text-center">5</td>

                          <td class="text-center">0</td>

                          <td class="text-center">3</td>

                          <td class="text-center font-bold">15</td>
                        </tr>

                        <tr class="border-b border-gray-200 hover:bg-white/60">
                          <td class="py-2">4</td>

                          <td class="py-2 flex items-center gap-3">
                            <img
                              src="https://upload.wikimedia.org/wikipedia/en/e/e1/Inter_Milan_2021_logo.svg"
                              class="w-6 h-6"
                              alt="Inter"
                            />

                            <span>Inter</span>
                          </td>

                          <td class="text-center">8</td>

                          <td class="text-center">4</td>

                          <td class="text-center">1</td>

                          <td class="text-center">3</td>

                          <td class="text-center font-bold">13</td>
                        </tr>

                        <tr class="hover:bg-white/60">
                          <td class="py-2">5</td>

                          <td class="py-2 flex items-center gap-3">
                            <img
                              src="https://upload.wikimedia.org/wikipedia/en/5/5b/US_Sassuolo_Calcio_logo.svg"
                              class="w-6 h-6"
                              alt="Sassuolo"
                            />

                            <span>Sassuolo</span>
                          </td>

                          <td class="text-center">8</td>

                          <td class="text-center">4</td>

                          <td class="text-center">1</td>

                          <td class="text-center">3</td>

                          <td class="text-center font-bold">13</td>
                        </tr>
                      </tbody>
                    </table>
                  </div>
                </div>
              </div>

              <!-- RIGHT: Stats, Game Statistic, Reminder -->

              <div class="flex flex-col gap-6">
                <!-- Game Statistic -->

                <div class="card">
                  <div class="flex justify-between items-center mb-3">
                    <h3 class="text-lg font-bold">Games statistic</h3>

                    <a href="#" class="text-sm text-teal-600 font-semibold">View all statistic</a>
                  </div>

                  <!-- segmented bar matching image: victories (teal), draws (gray), lost (pink) -->

                  <div class="seg-wrap w-full rounded-full mt-2" aria-hidden>
                    <!-- Victories 75% -->

                    <div
                      class="seg"
                      style="
                        left: 0;

                        width: 75%;

                        background: linear-gradient(90deg, #0ea5a4, #06b6d4);
                      "
                    ></div>

                    <!-- Draws 10% -->

                    <div
                      class="seg"
                      style="
                        left: 75%;

                        width: 10%;

                        background: linear-gradient(90deg, #d1d5db, #9ca3af);
                      "
                    ></div>

                    <!-- Lost 15% -->

                    <div
                      class="seg"
                      style="
                        left: 85%;

                        width: 15%;

                        background: linear-gradient(90deg, #f9a8d4, #f472b6);
                      "
                    ></div>
                  </div>

                  <div class="flex justify-between mt-3 text-sm text-gray-700 font-medium">
                    <span>PL 8</span>

                    <span>Victories 6</span>

                    <span>Draws 1</span>

                    <span>Lost 1</span>
                  </div>
                </div>

                <!-- Small Stats grid -->

                <div class="grid grid-cols-2 gap-3">
                  <div class="card p-3 text-center">
                    <div class="text-xs text-gray-500">Possession</div>

                    <div class="text-2xl font-bold">65%</div>

                    <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                      <div class="h-2 rounded-full" style="width: 65%; background: #10b981"></div>
                    </div>
                  </div>

                  <div class="card p-3 text-center">
                    <div class="text-xs text-gray-500">Overall price</div>

                    <div class="text-2xl font-bold">$690.2m</div>

                    <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                      <div class="h-2 rounded-full" style="width: 100%; background: #14b8a6"></div>
                    </div>
                  </div>

                  <div class="card p-3 text-center">
                    <div class="text-xs text-gray-500">Transfer budget</div>

                    <div class="text-2xl font-bold">$240.6m</div>

                    <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                      <div class="h-2 rounded-full" style="width: 75%; background: #fb923c"></div>
                    </div>
                  </div>

                  <div class="card p-3 text-center">
                    <div class="text-xs text-gray-500">Average score</div>

                    <div class="text-2xl font-bold">7.2</div>

                    <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
                      <div class="h-2 rounded-full" style="width: 72%; background: #60a5fa"></div>
                    </div>
                  </div>
                </div>

                <!-- Reminder -->

                <div
                  class="rounded-xl p-4 shadow-xl bg-gradient-to-r from-teal-600 to-green-400 text-white flex items-center justify-between"
                >
                  <div>
                    <div class="font-bold text-lg">Don't forget</div>

                    <div class="font-semibold text-sm mt-1">Setup training for next week</div>

                    <div class="text-xs mt-1">
                      Go to training center to plan tactical drills and recovery session
                    </div>
                  </div>

                  <div class="flex flex-col items-center gap-3">
                    <div
                      class="w-16 h-16 rounded-lg bg-white/20 flex items-center justify-center text-2xl"
                    >
                      🎯
                    </div>

                    <button
                      class="bg-white text-teal-700 px-3 py-1 rounded-lg font-semibold text-sm"
                    >
                      Go to training center
                    </button>
                  </div>
                </div>
              </div>
            </div>

            <!-- FOOTER -->

            <div class="mt-6 text-center text-xs text-gray-600">
              © 2025 Trinita Dashboard — Triwahyuni Vanisa Akili
            </div>
          </main>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>
