```html
<div class="QuestionDetails__container transition-opacity delay-150">
   <div class="QuestionDetails__contents flow">
      <div class="flex items-center gap-4">
         <h1 class="QuestionMetadata__h1 my-0 flex flex-grow items-center gap-4 text-3xl">
            Recommendation System
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 16 16" class="QuestionTitle__lock-icon">
               <path stroke="currentColor" stroke-miterlimit="10" stroke-width="2" d="M8 1.38a3.034 3.034 0 0 1 3.034 3.034v2.483H4.967V4.414A3.034 3.034 0 0 1 8 1.379Z"></path>
               <path fill="currentColor" d="M3.31 6.345h9.38a1.103 1.103 0 0 1 1.103 1.103v6.07a1.103 1.103 0 0 1-1.103 1.103H3.31a1.103 1.103 0 0 1-1.103-1.104V7.448A1.103 1.103 0 0 1 3.31 6.345"></path>
            </svg>
         </h1>
         <div class="Dropdown__container">
            <button type="button" aria-label="Share" class="Dropdown__toggle  Dropdown__toggle--border-0">
               <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 24 24">
                  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m8.59 13.51 6.83 3.98m-.01-10.98-6.82 3.98M21 5a3 3 0 1 1-6 0 3 3 0 0 1 6 0M9 12a3 3 0 1 1-6 0 3 3 0 0 1 6 0m12 7a3 3 0 1 1-6 0 3 3 0 0 1 6 0"></path>
               </svg>
            </button>
         </div>
         <button type="button" class="BookmarkButton__button" aria-label="Bookmark">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 24 24" class="BookmarkButton__icon ">
               <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 21-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path>
            </svg>
         </button>
      </div>
      <p class="QuestionMetadata__date">Last Updated: January 2026</p>
      <div class="QuestionMetadata__metadata my-4">
         <div class="QuestionDifficulty__container">
            <span class="QuestionDifficulty QuestionDifficulty--medium">
               <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 24 24" class="text-base">
                  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m7 13 5 5 5-5M7 6l5 5 5-5"></path>
               </svg>
               Medium
            </span>
            <span class="QuestionDifficulty__reason"><span class="QuestionDifficulty__reason-text">The difficulty is Medium, because the solution involves complex logic that requires joining multiple datasets and applying conditions to compare and filter results. This multi-step process entails identifying relationships between various entities and ensuring that users are recommended pages that none of their friends follow, adding layers of complexity to the task.</span></span>
         </div>
         <span>ID 2081</span>
         <div class="ml-auto flex gap-3">
            <button type="button" aria-label="Upvote" class="p-2 transition-colors hover:text-neutral-300 disabled:text-neutral-400 dark:disabled:text-neutral-500">
               <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-thumbs-up" aria-hidden="true">
                  <path d="M7 10v12"></path>
                  <path d="M15 5.88 14 10h5.83a2 2 0 0 1 1.92 2.56l-2.33 8A2 2 0 0 1 17.5 22H4a2 2 0 0 1-2-2v-8a2 2 0 0 1 2-2h2.76a2 2 0 0 0 1.79-1.11L12 2a3.13 3.13 0 0 1 3 3.88Z"></path>
               </svg>
            </button>
            <span class="py-2">204</span>
            <button type="button" aria-label="Downvote" class="p-2 transition-colors hover:text-neutral-300 disabled:text-neutral-400 dark:disabled:text-neutral-500">
               <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-thumbs-down" aria-hidden="true">
                  <path d="M17 14V2"></path>
                  <path d="M9 18.12 10 14H4.17a2 2 0 0 1-1.92-2.56l2.33-8A2 2 0 0 1 6.5 2H20a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2h-2.76a2 2 0 0 0-1.79 1.11L12 22a3.13 3.13 0 0 1-3-3.88Z"></path>
               </svg>
            </button>
         </div>
      </div>
      <div class="QuestionMetadata__question text-sm">
         <p>You are given the list of Facebook friends and the list of Facebook pages that users follow. Your task is to create a new recommendation system for Facebook. For each Facebook user, find pages that this user doesn't follow but at least one of their friends does. Output the user ID and the ID of the page that should be recommended to this user.</p>
      </div>
      <div>
         <h3 class="font-bold">Tables</h3>
         <div class="flex flex-wrap gap-2">
            <div class="QuestionPane__question-data QuestionPane__question-data--tables">users_friends</div>
            <div class="QuestionPane__question-data QuestionPane__question-data--tables">users_pages</div>
         </div>
      </div>
      <div></div>
      <div data-slot="accordion" data-orientation="vertical">
         <div data-state="open" data-orientation="vertical" data-slot="accordion-item" class="border-b last:border-b-0">
            <h3 data-orientation="vertical" data-state="open" class="my-0 flex">
               <button type="button" aria-controls="radix-_r_5_" aria-expanded="true" data-state="open" data-orientation="vertical" id="radix-_r_4_" data-slot="accordion-trigger" class="focus-visible:border-ring focus-visible:ring-ring/50 flex flex-1 items-start gap-4 rounded-md py-4 text-left text-sm outline-none transition-all hover:underline focus-visible:ring-[3px] disabled:pointer-events-none disabled:opacity-50 [&amp;[data-state=open]&gt;svg]:rotate-180 justify-start font-normal text-neutral-500" data-radix-collection-item="">
                  More about this question
                  <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chevron-down text-muted-foreground pointer-events-none size-4 shrink-0 translate-y-0.5 transition-transform duration-200" aria-hidden="true">
                     <path d="m6 9 6 6 6-6"></path>
                  </svg>
               </button>
            </h3>
            <div data-state="open" id="radix-_r_5_" role="region" aria-labelledby="radix-_r_4_" data-orientation="vertical" data-slot="accordion-content" class="data-[state=closed]:animate-accordion-up data-[state=open]:animate-accordion-down overflow-hidden text-sm" style="--radix-accordion-content-height: var(--radix-collapsible-content-height); --radix-accordion-content-width: var(--radix-collapsible-content-width); --radix-collapsible-content-height: 410px; --radix-collapsible-content-width: 797px;">
               <div class="pb-4 pt-0">
                  <h3 class="font-bold">Companies</h3>
                  <div class="my-4 flex flex-wrap gap-2">
                     <div class="QuestionMetadata__pill [--bg-color-primary:var(--color-alert)]">Meta</div>
                  </div>
                  <h3 class="font-bold">Job Positions</h3>
                  <div class="my-4 flex flex-wrap gap-2">
                     <div class="QuestionMetadata__pill">Data Engineer</div>
                     <div class="QuestionMetadata__pill">Data Scientist</div>
                     <div class="QuestionMetadata__pill">BI Analyst</div>
                     <div class="QuestionMetadata__pill">Data Analyst</div>
                     <div class="QuestionMetadata__pill">ML Engineer</div>
                  </div>
                  <h3 class="font-bold">Topic Family</h3>
                  <div class="my-4 flex flex-wrap gap-2">
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Column Manipulation</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Data Cleaning</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">DataFrame Operations</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Data Manipulation &amp; Wrangling</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Data Retrieval Basics</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Filtering Data</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Joins Merging</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Joins &amp; Merging</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Joins &amp; Set Operations</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Join Types</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Merge Operations</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Null Handling</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">Tidyverse Essentials</div>
                  </div>
                  <h3 class="font-bold">Topic Functions</h3>
                  <div class="my-4 flex flex-wrap gap-2">
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">anti_join()</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">distinct()</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">drop_duplicates()</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">inner_join()</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">isna()</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">merge()</div>
                     <div class="QuestionMetadata__pill [--bg-color-primary:#8338e31a]">select()</div>
                  </div>
               </div>
            </div>
         </div>
      </div>
      <hr>
      <div class="QuestionHints__header flex gap-2">
         <button class="Button inline-flex w-full items-center justify-center gap-2 rounded-full font-bold TitleToggle__button" data-variant="outline" data-size="rectangle" disabled="">
            Hints
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 16 16">
               <path stroke="currentColor" stroke-miterlimit="10" stroke-width="2" d="M8 1.38a3.034 3.034 0 0 1 3.034 3.034v2.483H4.967V4.414A3.034 3.034 0 0 1 8 1.379Z"></path>
               <path fill="currentColor" d="M3.31 6.345h9.38a1.103 1.103 0 0 1 1.103 1.103v6.07a1.103 1.103 0 0 1-1.103 1.103H3.31a1.103 1.103 0 0 1-1.103-1.104V7.448A1.103 1.103 0 0 1 3.31 6.345"></path>
            </svg>
         </button>
         <button class="Button inline-flex w-full items-center justify-center gap-2 rounded-full font-bold TitleToggle__button" data-variant="outline" data-size="rectangle" disabled="">
            Expected Output
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 16 16">
               <path stroke="currentColor" stroke-miterlimit="10" stroke-width="2" d="M8 1.38a3.034 3.034 0 0 1 3.034 3.034v2.483H4.967V4.414A3.034 3.034 0 0 1 8 1.379Z"></path>
               <path fill="currentColor" d="M3.31 6.345h9.38a1.103 1.103 0 0 1 1.103 1.103v6.07a1.103 1.103 0 0 1-1.103 1.103H3.31a1.103 1.103 0 0 1-1.103-1.104V7.448A1.103 1.103 0 0 1 3.31 6.345"></path>
            </svg>
         </button>
      </div>
      <hr>
      <div class="QuestionTables__header">
         <h3 class="QuestionTables__table-name">users_friends</h3>
         <button class="Button inline-flex w-full items-center justify-center gap-2 rounded-full font-bold px-3 py-2 text-sm QuestionTables__preview-btn QuestionTables__preview-btn--active" data-variant="outline" data-size="tiny">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 24 24">
               <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8"></path>
               <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15a3 3 0 1 0 0-6 3 3 0 0 0 0 6"></path>
            </svg>
            Preview
         </button>
      </div>
      <div>
         <div class="mt-0 overflow-x-auto">
            <div style="width: 782px; min-height: 20px;"></div>
         </div>
         <div class="ResultsTable__container QuestionTables__preview-table">
            <table class="ResultsTable__table">
               <thead>
                  <tr class="ResultsTable__header-row">
                     <th class="ResultsTable__header-cell">user_id</th>
                     <th class="ResultsTable__header-cell">friend_id</th>
                  </tr>
               </thead>
               <tbody>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">1</td>
                     <td class="ResultsTable__cell">2</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">1</td>
                     <td class="ResultsTable__cell">4</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">1</td>
                     <td class="ResultsTable__cell">5</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">1</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">3</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">4</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">5</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">3</td>
                     <td class="ResultsTable__cell">2</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">4</td>
                     <td class="ResultsTable__cell">1</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">4</td>
                     <td class="ResultsTable__cell">2</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">5</td>
                     <td class="ResultsTable__cell">1</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">5</td>
                     <td class="ResultsTable__cell">2</td>
                  </tr>
               </tbody>
            </table>
         </div>
      </div>
      <div class="DatasetTableTypes__container grid auto-rows-max grid-cols-2 gap-3 rounded-md px-5 py-4"><span class="font-bold">friend_id:</span><span>bigint</span><span class="font-bold">user_id:</span><span>bigint</span></div>
      <div class="QuestionTables__header">
         <h3 class="QuestionTables__table-name">users_pages</h3>
         <button class="Button inline-flex w-full items-center justify-center gap-2 rounded-full font-bold px-3 py-2 text-sm QuestionTables__preview-btn QuestionTables__preview-btn--active" data-variant="outline" data-size="tiny">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" fill="none" viewBox="0 0 24 24">
               <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8"></path>
               <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15a3 3 0 1 0 0-6 3 3 0 0 0 0 6"></path>
            </svg>
            Preview
         </button>
      </div>
      <div>
         <div class="mt-0 overflow-x-auto">
            <div style="width: 782px; min-height: 20px;"></div>
         </div>
         <div class="ResultsTable__container QuestionTables__preview-table">
            <table class="ResultsTable__table">
               <thead>
                  <tr class="ResultsTable__header-row">
                     <th class="ResultsTable__header-cell">user_id</th>
                     <th class="ResultsTable__header-cell">page_id</th>
                  </tr>
               </thead>
               <tbody>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">1</td>
                     <td class="ResultsTable__cell">21</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">1</td>
                     <td class="ResultsTable__cell">25</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">25</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">23</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">24</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">28</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">2</td>
                     <td class="ResultsTable__cell">21</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">3</td>
                     <td class="ResultsTable__cell">25</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">3</td>
                     <td class="ResultsTable__cell">24</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">5</td>
                     <td class="ResultsTable__cell">23</td>
                  </tr>
                  <tr class="ResultsTable__row ">
                     <td class="ResultsTable__cell">5</td>
                     <td class="ResultsTable__cell">28</td>
                  </tr>
               </tbody>
            </table>
         </div>
      </div>
      <div class="DatasetTableTypes__container grid auto-rows-max grid-cols-2 gap-3 rounded-md px-5 py-4"><span class="font-bold">page_id:</span><span>bigint</span><span class="font-bold">user_id:</span><span>bigint</span></div>
      <hr>
   </div>
</div>
```
