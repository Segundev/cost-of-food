<script>
	import Chart from './Chart.svelte';
	import { chartData } from '../lib/chartType';
	import SubHeader from './subHeader.svelte';
</script>

<section>
	<p>
		As the year comes to an end, it is marked by widespread celebrations, and one popular avenue for
		celebrating is through the enjoyment of well-prepared homemade food. The Christian community
		celebrated Christmas with the customary inclusion of chicken, a ritual observed on the 25th.
		Meanwhile, a common holiday custom involves families going on trips and getting together with
		family members. But as we all know, it costs a lot to be outside.
	</p>
	<p>
		When examining the data provided by the National Bureau of Statistics concerning our consumption
		patterns in 2019, we consumed less homemade food. Approximately 20 percent of our total food
		expenditure was allocated to meals consumed outside the home. Even dedicating more time to
		cooking at home or opting for nearby restaurants does not shield individuals from the escalating
		trend in food prices. Over the past year, food prices have witnessed a significant doubling, and
		as of November, food inflation stands at 31.52 percent, marking the highest rate since 1996.
	</p>
</section>

<section>
	<SubHeader>Christmas is expensive</SubHeader>
	<p>
		Mr. Dayo, an estate manager who is a family man with a wife and son, celebrated his third
		Christmas with his new family. During our discussion, he emphasized the importance of
		reevaluating the choice between purchasing a live chicken or opting for the more economical
		alternative of frozen chicken.
	</p>
	<Chart chartName={chartData[5].chartName} altText={chartData[5].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
	<p>
		He pointed out that the decision largely hinges on the cost of each item. In a comparative
		analysis with the previous year, the cost of frozen chicken has witnessed a substantial
		increase. While a kilogram of frozen chicken was priced at ₦1500 in the past, it is currently
		being retailed for ₦3000. Furthermore, a three- to four-month-old chicken is now commanding a
		price range of ₦7500 to ₦10,000. Common practice now is to see households rear their chickens
		close to any major festive period.
	</p>
	<p>
		With everyone trying to be economical and cut costs, the reality of things pushing individuals
		to cultivate what to eat, and as previously advised by our former President Buhari for all to
		engage in farming, we all definitely can't be farmers.
	</p>
</section>

<section>
	<SubHeader>Cost of farming has increased</SubHeader>
	<p>
		Let’s dive a bit into poultry farming. The primary driver of the increase in the price of
		poultry meat is the escalating cost of raising these birds. In January, a kilogram of poultry
		feed was retailed at ₦400, but it is currently being sold for ₦800, with a 25-kilogram bag
		commanding a price of ₦14,000. Conducting a cost analysis reveals that the 25-kilogram bag can
		sustain less than three birds until full maturity.
	</p>
	<Chart chartName={chartData[9].chartName} altText={chartData[9].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
	<p>
		Majority of the components used in feed production can be sourced locally. Maize, soybean,
		wheat, rice bran, and limestone are all cultivated across the country. Nigeria is the
		second-largest producer of maize in Africa and the 14th-largest globally. While maize is
		extensively grown across the nation, the primary production centers are in Borno, Niger,
		Plateau, Katsina, Gombe, Bauchi, Kogi, Kaduna, Oyo, and Taraba states. These top ten
		maize-producing states account for nearly two-thirds (64%) of the total maize production in
		Nigeria. Despite the substantial local production, the demand for maize still surpasses the
		supply, resulting in an annual demand gap of approximately 4 million metric tons.
	</p>
	<p>
		If major materials can be sourced within the country, what might be the cause of the current
		challenges? Mr. Tobi, the owner of Topfeeds, a feed manufacturer in Osogbo, shed light on a
		significant contributing factor – the price of diesel.
	</p>
	<p>
		When probed further about the source of his supplies, despite being located in Osogbo, he
		clarified that he obtains all his supplies within the state and has consistently maintained an
		uninterrupted flow. However, on certain occasions, he has resorted to ordering maize from Kano.
	</p>
	<p>
		He emphasized how the surge in diesel prices directly impacts the cost of poultry feed. Diesel
		is primarily used to fuel the majority of trucks and buses involved in transporting goods from
		the North. Additionally, the machines used in the production of these feeds are powered by
		diesel.
	</p>
</section>
<section>
	<SubHeader>Diesel a major reason why food is expensive</SubHeader>
	<p>
		Nigeria is confronted with a multifaceted energy challenge. Electricity, which should be the
		primary power source, is notably absent. We won’t dwell more on this issue but shift our focus
		to the alternative, which is crude oil products.
	</p>
	<p>
		As a major producer of crude oil, our economic realities differ from the anticipated benefits of
		being the third-largest oil-producing country in Africa. Despite exporting crude oil, we find
		ourselves importing refined products, a situation expected to be addressed by the Dangote
		Refinery and the recently renovated Port Harcourt Refinery.
	</p>
	<p>
		Global events such as the conflict between Russia and Ukraine, it was expected that the demand
		shortage from Russia would be compensated by other oil-producing countries. However, in recent
		months, Nigeria's oil production capacity has dwindled, falling short of the 1.74 million
		barrels per day quota allocated by OPEC and significantly below the 1.69 million barrels per day
		assumed in the 2023 budget. A major contributing factor is vandalism and theft.
	</p>
	<Chart chartName={chartData[3].chartName} altText={chartData[3].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
	<p>
		As mentioned earlier, we both produce and import refined products, including PMS, diesel, jet
		fuel, and even cooking gas, with at least 50 percent of our consumption being imported. Prior to
		the removal of the fuel subsidy, the government bore the burden of the difference between
		international prices and the pump price. However, this became unsustainable, leading President
		Tinubu to declare in his inaugural speech that the government would no longer shoulder this
		burden. Consequently, prices surged, with PMS averaging ₦200 in November last year and now
		selling for ₦650, while diesel, previously at ₦810, has risen to ₦1060.
	</p>
	<Chart chartName={chartData[2].chartName} altText={chartData[2].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
</section>
<section>
	<SubHeader>Border Closure and Exchange Rate and its negative effect</SubHeader>
	<p>
		Some economic policies, aimed at protecting local industries and promoting domestic production,
		have contributed to the rise in food costs. The prohibition on importing certain items and the
		border closure to favor homemade agricultural production have resulted in increased prices due
		to a supply shortage.
	</p>
	<p>
		In light of the reality of declining forex earnings, the Central Bank of Nigeria (CBN) has faced
		challenges in maintaining the dollar at a reasonable rate. Previously, we operated under a
		system with various windows and a fixed peg, but the shift to a market-driven rate, determined
		by demand and supply, was adopted due to insufficient supply from oil sales, diaspora
		remittances, and foreign direct portfolio investments. The government found the previous
		multi-window regime to be costly, prompting the adoption of the new policy.
	</p>
	<Chart chartName={chartData[5].chartName} altText={chartData[5].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
	<p>
		However, the persisting challenge lies in the fact that low forex earnings have not been able to
		meet the demands for dollars.
	</p>
</section>
<section>
	<SubHeader>Other foods items are expensive too</SubHeader>
	<p>
		The same issue elucidated in the feeds and poultry analogy, as explained above, resonates with
		other food and non-food items. Staple food items, extensively consumed by Nigerians, have
		witnessed a doubling in prices since 2020. For instance, a bag of rice, which was priced at
		₦12,000 in 2016, now commands a staggering ₦55,000.
	</p>
	<Chart chartName={chartData[7].chartName} altText={chartData[7].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
	<p>
		Similarly, alternatives to poultry meat, such as beef and fish, have also seen significant
		increases. The cost of beef, which was ₦1,000 in January 2021, now averages ₦2,500. Likewise,
		the price of fish, specifically a titus fish, has surged from ₦1,050 in January 2021 to the
		current price of ₦2,000.
	</p>
	<p>
		Basic breakfast essentials like bread and eggs have become cost-prohibitive for many families. A
		crate of eggs, priced at ₦500 in 2021, has now skyrocketed to ₦2,500. Similarly, a sliced loaf
		of bread, which was sold for ₦300 in 2017, now commands about ₦1,000.
	</p>
	<p>
		Palm oil and vegetable oil, crucial items that were initially banned before the removal in
		October, have also experienced a doubling in price. A liter of vegetable oil, formerly sold for
		₦650 in 2021, is now priced at ₦1,500. Likewise, palm oil has seen a significant increase from
		₦550 in 2021 to ₦1,350 in October.
	</p>
</section>
<section>
	<SubHeader>How would households cope?</SubHeader>
	<p>
		Nigerians collectively spent ₦22 trillion on food expenditures, with 56 percent of the country's
		total expenditure allocated to food. Breaking down food expenditure on a per capita basis, the
		average Nigerian spent ₦114,000 in 2019. This translates to an average monthly expenditure of
		₦9,500 and ₦300 per day on food. For reference, a loaf of unsliced bread is priced at around
		₦1,000.
	</p>
	<p>
		Consumer responses to price increases typically manifest in two ways: through the income effect,
		leading to a reduction in consumption, or the substitution effect, where consumers opt for more
		affordable alternatives.
	</p>
	<p>
		Income plays a pivotal role in this scenario, especially considering the relatively low earning
		power of Nigerians. With the minimum wage at ₦30,000, even those earning around ₦100,000
		experience limited purchasing power due to inflation. If we consider the earnings of ₦100,000 in
		2020, accounting for inflation reduces it to ₦86,000. Comparatively, given the current inflation
		rate, it is approximately ₦67,000.
	</p>
	<Chart chartName={chartData[1].chartName} altText={chartData[1].altText}
		>Chart showing the prices of meat between 2017 and 2023</Chart
	>
	<p>
		Data from 2019 reveals that when confronted with food insecurity, a majority of households lack
		effective coping mechanisms. Savings are the least relied upon, with households either
		maintaining the status quo and hoping for the best, reducing food consumption, or seeking
		assistance from friends and family. Nigerians remain optimistic, clinging to hope for a better
		future—this is our resilience.
	</p>
</section>
