<template>
  <div class="w-full flex flex-col items-start px-[20px] py-[50px] gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
    <div class="w-full border-b border-[#ccc] justify-center lg:justify-between pb-5 flex">
      <div class="hidden lg:flex items-center gap-4">
        <div class="flex flex-col text-[20px] font-semibold">
          <span>Download Paytm App</span>
          <span>to Pay from anywhere</span>
        </div>
        <nuxt-link to="/"
          class="bg-black flex gap-1 items-center px-3 pl-1 py-1 rounded-lg text-white border hover:border-black hover:bg-white hover:text-black transition-all duration-300">
          <Icon class="text-[35px]" name="ic:round-apple" />
          <div class="flex flex-col text-[20px]">
            <span class="text-[11px] tracking-wide">Download on the</span>
            <span>App Store</span>
          </div>
        </nuxt-link>
        <nuxt-link to="/"
          class="bg-black flex gap-1 items-center px-3 pl-1 py-1 rounded-lg text-white border hover:border-black hover:bg-white hover:text-black transition-all duration-300">
          <Icon class="text-[35px]" name="ion:logo-google-playstore" />
          <div class="flex flex-col text-[20px]">
            <span class="text-[11px] tracking-wide">GET IT ON</span>
            <span>Google Play</span>
          </div>
        </nuxt-link>
      </div>
      <div class="flex text-[28px] justify-center items-center gap-6 text-gray-500">
        <nuxt-link to="/">
          <Icon name="ri:twitter-x-line" />
        </nuxt-link>
        <nuxt-link to="/">
          <Icon name="uim:instagram" />
        </nuxt-link>
        <nuxt-link to="/">
          <Icon name="gg:facebook" />
        </nuxt-link>
        <nuxt-link to="https://github.com/">
          <Icon name="ri:github-fill" />
        </nuxt-link>
        <nuxt-link to="https://www.linkedin.com/">
          <Icon name="ri:linkedin-box-line" />
        </nuxt-link>
      </div>
    </div>
    <div class="w-full">
      <Acord title="Investor Relations" :initialOpen="openAcord === 1" @toggle="toggleAccord(1)">
        <ul class="w-full flex flex-col justify-around">
          <li>
            <InneraccordAccordion title="Home" :initialOpen="innerAcord === 1" @toggle="toggleInnerAcord(1)">
              <ul
                class="flex flex-col sm:flex-grow sm:justify-start gap-5 px-2 py-3 transition-all duration-300 text-[#ccc] text-[13.5px] tracking-wider">
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]"
                    to="/">Overview</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Our
                    Business</nuxt-link>
                </li>
              </ul>
            </InneraccordAccordion>
          </li>
          <li>
            <InneraccordAccordion title="Financials" :initialOpen="innerAcord === 2" @toggle="toggleInnerAcord(2)">
              <ul
                class="flex flex-col gap-5 px-2 py-3 transition-all duration-300 text-[#ccc] text-[13.5px] tracking-wider">
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Financial
                    Results</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Annual
                    Report & other documents</nuxt-link>
                </li>
              </ul>
            </InneraccordAccordion>
          </li>
          <li>
            <InneraccordAccordion title="Fillings & Releases" :initialOpen="innerAcord === 3"
              @toggle="toggleInnerAcord(3)">
              <ul
                class="flex flex-col gap-5 px-2 py-3 transition-all duration-300 text-[#ccc] text-[13.5px] tracking-wider">
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">All Stock
                    Exchange Fillings</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Press
                    Releases</nuxt-link>
                </li>
              </ul>
            </InneraccordAccordion>
          </li>
          <li>
            <InneraccordAccordion title="News & Events" :initialOpen="innerAcord === 4" @toggle="toggleInnerAcord(4)">
              <ul
                class="flex flex-col gap-5 px-2 py-3 transition-all duration-300 text-[#ccc] text-[13.5px] tracking-wider">
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Media
                    Articles</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]"
                    to="/">Awards</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]"
                    to="/">Videos</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]"
                    to="/">Blog</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Press
                    Kit</nuxt-link>
                </li>
              </ul>
            </InneraccordAccordion>
          </li>
          <li>
            <InneraccordAccordion title="Corporate Governance" :initialOpen="innerAcord === 5"
              @toggle="toggleInnerAcord(5)">
              <ul
                class="flex flex-col gap-5 px-2 py-3 transition-all duration-300 text-[#ccc] text-[13.5px] tracking-wider">
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Board of
                    Directors & Committiees</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">General
                    Meetings</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]"
                    to="/">CSR</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">ESG
                    Profiles</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Policies &
                    Other Documents</nuxt-link>
                </li>
              </ul>
            </InneraccordAccordion>
          </li>
          <li>
            <InneraccordAccordion title="Resources" :initialOpen="innerAcord === 6" @toggle="toggleInnerAcord(6)">
              <ul
                class="flex flex-col gap-5 px-2 py-3 transition-all duration-300 text-[#ccc] text-[13.5px] tracking-wider">
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Investor
                    Relations Contacts</nuxt-link>
                </li>
                <li>
                  <nuxt-link class="hover:text-[#1d2c38] transition-all duration-300 hover:text-[14px]" to="/">Frequently
                    Asked Questions</nuxt-link>
                </li>
              </ul>
            </InneraccordAccordion>
          </li>
        </ul>
      </Acord>
      <Acord title="More about Paytm" :initialOpen="openAcord === 2" @toggle="toggleAccord(2)">
        <div class="text-xs">
          <h1 class="text-[#505050] font-semibold pb-1">Paytm - India's Most Popular Platform for Money Transfer, BHIM UPI
            Payments, Recharges and other online
            payments</h1>
          <p class="text-[#707070] py-[12px]">Paytm - India’s largest mobile e-commerce website is an ultimate destination
            for prompt
            <a href="https://paytm.com/recharge" class="text-[#00baf2]"> Online Recharge</a>, DTH, Data Card &amp; Metro
            Card Recharge and Mobile
            Bill Payment for Airtel, Aircel, BSNL, Idea, MTNL, Vodafone &amp; other operators for all the circles across
            India. Enjoy our online recharge and bill payment service along with best bonus packs of internet &amp;
            roaming within a jiffy.
          </p>
          <p class="text-[#707070] py-[12px]">Now you don’t have to look at various websites to find the best
            entertainment option in your city. You can
            book movie tickets, event tickets and travel tickets within minutes on Paytm.com. Paytm login is very easy on
            the
            <a href="https://paytm.com/download-paytm-app" class="text-[#00baf2]">Paytm app</a> and Paytm website. Just
            enter your number and
            Password/OTP to login and process all the transactions instantly on Paytm.
          </p>
          <h2 class="font-semibold pb-1 text-[#505050]">Mobile Recharge - Airtel, Vodafone, Idea, Jio, BSNL, MTNL, and
            More </h2>
          <p class="text-[#707070] py-[12px]">Now making an online recharge has become very easy and safe with your Paytm
            account on Paytm.com.
            Effortlessly make payments through our safe methods, processed through secured gateways for
            <a class="text-[#00baf2]" href="https://paytm.com/recharge/airtel-prepaid-mobile-online-recharge"> Airtel
              Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/recharge/jio-prepaid-mobile-online-recharge"> Jio
              Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/recharge/vodafone-idea-prepaid-mobile-online-recharge">
              Vodafone Idea Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/recharge/mtnl-prepaid-mobile-online-recharge"> MTNL
              Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/recharge/bsnl-prepaid-mobile-online-recharge"> BSNL
              Recharge</a>. Paytm also
            provide you with exciting cashback and offers on Paytm
          </p>
          <p class="text-[#707070] py-[12px]">All The Latest Plans And Packs For Your Mobile Recharge- Paytm makes it very
            easier for you to make recharge
            online with Paytm. You can browse all the latest recharge plans and offers right on Paytm itself. More than
            that, Paytm.com or Paytm app fetches your operator and circle automatically as soon as you enter your number,
            making the process faster and easier for you.</p>
          <h2 class="font-semibold pb-1 text-[#505050]">Online Shopping- Find Best Deals Online On Groceries, Appliances
            And Latest Smart Phones at Paytm </h2>
          <p class="text-[#707070] py-[12px]">Paytm Mall Maha Shopping Festival Sale is back this festive season. Shop on
            Paytm Mall and enjoy the best
            ever online Diwali sale you can come across. With a vibrant range of products from electronic gadgets, mobiles
            and appliances to fashion accessories and footwear collections at unbelievable prices, this online sale is
            going to be the year’s best shopping experience!</p>
          <p class="text-[#707070] py-[12px]">Tech Fanatics, if you are eager to buy the best
            <a class="text-[#00baf2]" href="https://paytmmall.com/mobiles-tablets-clpid-6942"> mobile</a> phones then here
            is an ultimate mobile
            destination for you. Discover the wide selection of mobiles like VIVO V15 Pro, Oppo F11 Pro, Samsung Galaxy
            A50, iPhone X, Redmi Y2, Lenovo K8 Note, VIVO Y55S, Redmi Note 6 Pro so on that offers the perfect combination
            of performance and exciting features. There is a lot more for you to explore, check out the exhaustive
            collection of the latest smartphones at great discounts and Cashbacks on Paytm Mall. Add a brand new vehicle
            to your collection, enjoy the exclusive online pre-booking service for
            <a class="text-[#00baf2]" href="https://paytmmall.com/cars-bikes-clpid-836"> new cars &amp; bikes</a> at
            Paytm. Be the first one to
            bring home the newly launched automobile, forget sweating for owning the latest car &amp; bike in the town.
            With Paytm, you can make pre-booking online for cars &amp; bikes in seconds along with exclusive offers that
            are especially for you.
          </p>
          <p class="text-[#707070] py-[12px]">Cashback would be added as Paytm Cash, which is One97 Communications Ltd.
            loyalty program. It can be used to
            pay for goods &amp; services sold by merchants that accept ‘Pay with Paytm’.</p>
          <p class="text-[#707070] py-[12px]">Grab jaw-dropping
            <a class="text-[#00baf2]" href="https://paytm.com/coupons">Paytm Coupons</a>, Deals, Discounts &amp; Cashback
            Offers while shopping,
            who wouldn’t love to shop at discounted prices Paytm presents several
            <a class="text-[#00baf2]" href="https://paytm.com/offer/">offers</a> across a huge range of products under our
            stimulating stores.
            Shop more &amp; save even more at Sunday Bazaar, Bargain Bazaar and Under 199 stores. Double the joy of
            weekend shopping, avail electrifying offers at our Sunday Bazaar, this is surely going to make your Sunday
            more amazing Buy your favourites at the lowest price possible with tons of discounts at Under 199 Store and
            shop more with smartness from our irresistible Bargain Bazaar.
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Online Tickets - Flight Tickets, Train Tickets And Bus Tickets
            with Great Ease</h2>
          <p class="text-[#707070] py-[12px]">Save money and time by booking your travel tickets on Paytm. You can find
            <a class="text-[#00baf2]" href="https://paytm.com/flights">cheap flight tickets</a>, train tickets and bus
            tickets on Paytm. Compare
            the prices, get schedules, pick the best-suited seat and experience easy ticket booking services online. You
            can also save money on your travel by applying promo codes on flights, buses &amp; trains to get cashback in
            your Paytm wallet on your travel tickets.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Flight Tickets</span>- Make your flight booking online on Paytm to
            find cheap flight tickets and
            <a class="text-[#00baf2]" href="https://paytm.com/flights">flight tickets </a>offers. Just enter your boarding
            and destination city
            to know all the flight tickets prices for both
            <a class="text-[#00baf2]" href="https://paytm.com/flights">domestic flights </a>and
            <a class="text-[#00baf2]" href="https://paytm.com/flights/international-tickets">international flights</a>.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Train Ticket Booking</span>-
            <a class="text-[#00baf2]" href="https://paytm.com/train-tickets/pnr-status">Check PNR status</a>, find train
            schedule and
            <a class="text-[#00baf2]" href="https://paytm.com/train-tickets/seat-availability">get train seat
              availability</a> for your online
            <a class="text-[#00baf2]" href="https://paytm.com/train-tickets"> train ticket bookings</a>. Just enter your
            boarding and destination
            station or city to know all the train ticket prices. Make instant train reservation through Paytm and save
            money with cashback.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Bus Tickets</span>- Make fast online
            <a class="text-[#00baf2]" href="https://paytm.com/bus-tickets"> bus ticket booking </a>for both AC and Non-AC
            buses, private and
            government buses on Paytm. Find all the buses and timings along with
            <a class="text-[#00baf2]" href="https://paytm.com/offer/bus-tickets/"> bus ticket offers</a> for your bus
            tickets.
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Mobile, DTH and Data Card Recharge &amp; Payment On-The-Go</h2>
          <p class="text-[#707070] py-[12px]">No need to rush to the market for
            <a class="text-[#00baf2]" href="https://paytm.com/dth-recharge">DTH Recharge</a> or
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment">Mobile Bill Payment</a>, just login to
            Paytm and make
            immediate payments. Cherish your experience with exciting Cashback and Discounts on every recharge or bill
            payment you make with us. Our online recharge and bill payment service is a one-stop solution for fast &amp;
            easy Prepaid Mobiles, DTH &amp; Data Card recharge and Postpaid Mobiles.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">DTH Recharge</span>- Make DTH recharge online and get DTH recharge
            offers on Paytm.
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment">Tata sky recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/dth-recharge/airtel-digital-tv">Airtel DTH recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/dth-recharge/airtel-digital-tv">Videocon D2H recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/dth-recharge/sun-direct">Sun Direct recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/dth-recharge/dish-tv">Dish TV recharge</a> and more on
            Paytm.com. Find all the
            latest DTH recharge offers and plans only on Paytm.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Data Card Recharge</span>- Get your
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-recharge/airtel">Airtel Data Card Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-recharge/vodafone">Vodafone Idea Data Card
              Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-recharge/jio">Jio Data Card Recharge</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-recharge/bsnl"> BSNL Data Card Recharge</a> and
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-recharge/mtnl">MTNL Data Card Recharge</a> now on
            Paytm.com and avail
            cashback by applying promo codes.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Data Card Bill Payment</span>: Pay your data card bills on your
            postpaid connection of
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-bill-payment/airtel">Airtel</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-bill-payment/airtel"> Idea</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/datacard-bill-payment/vodafone">Vodafone</a>.
          </p>
          <p class="text-[#707070] py-[12px]">Visit us and recharge your Prepaid Mobile, DTH and Data Card or Make
            Postpaid Mobile Bill Payments and other
            Utility Bill Payments in a click and indulge into an unbelievable
            <a class="text-[#00baf2]" href="https://paytmmall.com"> online shopping</a> experience.
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Buy FASTag Online And Move Quickly Through the Toll Lanes:</h2>
          <p class="text-[#707070] py-[12px]">Avoid long queues at the toll lanes and move quickly through them with the
            help of Paytm
            <a class="text-[#00baf2]" href="https://paytm.com/fastag"> FASTag</a>. It is very easy to buy FASTag for your
            vehicle at Paytm in
            just a few minutes. Order Toll-Tag now or just register for one at Paytm instantly and drive freely with the
            toll tags.
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Online Bill Payment Postpaid Bills, Quick Utility Bill, Insurance,
            Loan &amp; Education Fee Payment</h2>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Postpaid Bill Payment</span>- Mobile Post-paid bill payments for
            all the renowned operators such as
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment/airtel-postpaid"> Airtel</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment/vodafone-idea-postpaid"> Vodafone Idea
              Postpaid</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment/jio"> Jio</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment/bsnl-postpaid"> BSNL</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/mobile-bill-payment/mtnl-dolphin-postpaid"> MTNL </a>are
            available on Paytm.com.
          </p>
          <p class="text-[#707070] py-[12px]">Pay
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment">Electricity Bill</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment">Gas Bill</a> &amp; Water Bill instantly in
            just a few clicks
            Enjoy uncomplicated utility bill online payment service without even travelling to the stores at Paytm. We are
            no doubt a reliable platform for speedy electricity, gas &amp; water bill payment.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Electricity Bill Payment</span>- Pay your electricity bills online
            on Paytm.com and avoid waiting in the
            queues for hours with Paytm.com. Pay electricity bills in
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment/goa">Goa Electricity Bill
              Payment</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment/bihar"> Bihar Electricity Bill
              Payment</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment/haryana">Haryana Electricity Bill
              Payment</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment/maharashtra"> Maharashtra
              Electricity Bill Payment</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment/punjab">Punjab Electricity Bill
              Payment</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/electricity-bill-payment/telangana">Telangana Electricity
              Bill Payment</a> and many
            more cities.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Gas And Water Bill Payment</span>- Pay your water bills within
            seconds in of
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment/Delhi-Jal-Board-DJB"> Delhi Jal
              Board</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment">Indore Municipal Corporation</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment"> Gwalior Municipal Corporation</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment"> Bhopal Municipal Corporation</a>,
            <a class="text-[#00baf2]"
              href="https://paytm.com/water-bill-payment/bangalore-water-supply-and-sewerage-board-bwssb"> Bangalore
              Water Supply and Sewage Board</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment/Surat-Municipal-Corporation-Water"> Surat
              Municipal
              Corporation</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment/pune-municipal-corporation-water"> Pune
              Municipal
              Corporation</a>,
            <a class="text-[#00baf2]"
              href="https://paytm.com/water-bill-payment/nagpur-municipal-corporation-orange-city-water-nagpur"> Nagpur
              Municipal Corporation</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/water-bill-payment/uttarakhand-jal-sansthan"> Uttrakhand Jal
              Sansthan</a> and more.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Pay gas bills</span> of
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment/indraprastha-gas-limited"> Indraprastha Gas
              Limited</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment/gujarat-gas-limited"> Gujarat Gas
              Limited</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment/gujarat-gas-limited"> Adani Gas
              Limited</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment/Aavantika-Gas-Ltd"> Aavantika Gas
              Limited</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment/vadodara-gas-limited-vgl"> Vadodara Gas
              Limited</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/gas-bill-payment/maharashtra-natural-gas-limited-mngl">
              Maharashtra Natural Gas Ltd
            </a>and more.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Fee Payment, Metro Card Recharge, Insurance Premium and Gold
              Loan</span>- Forget those gigantic queues,
            <a class="text-[#00baf2]" href="https://paytm.com/education">pay admission fee </a>or registration fee for
            various Institutes,
            Schools &amp; Colleges online here and save your time. We ensure to provide you with a seamless and speedy
            service every time you visit us. Now you can also
            <a class="text-[#00baf2]" href="https://paytm.com/metro-card-recharge">recharge metro card </a>and instantly
            <a class="text-[#00baf2]" href="https://paytm.com/insurance-premium-payment"> pay insurance premium</a> &amp;
            gold loan online with
            Paytm through the comfort of wherever you are.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Landline And Broadband Bill Payment</span> - Pay landline and
            broadband bills of all the major operators
            such as
            <a class="text-[#00baf2]" href="https://paytm.com/landline-bill-payment/airtel">Airtel</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/landline-bill-payment/bsnl">BSNL</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/broadband-bill-payment/hathway-broadband"> Hathway</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/broadband-bill-payment/asianet-broadband">Asianet
              Broadband</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/broadband-bill-payment/alliance-broadband">Alliance
              Broadband</a>,
            <a class="text-[#00baf2]" href="https://paytm.com/broadband-bill-payment/Tata-Play-Fiber">Tata Play Fibre</a>
            and many more at
            Paytm.com.
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Mutual Fund Investments made Simple, Transparent and Accessible
            with Paytm Money</h2>
          <p class="text-[#707070] py-[12px]">Ab Mutual Funds ke liye bhi Paytm Karo. Presenting, Paytm Money - India's
            Most Sincere Wealth Adviser. You
            can now begin your
            <a class="text-[#00baf2]" href="https://www.paytmmoney.com/mutual-funds"> mutual fund</a> investment journey
            on the Paytm Money App
            with 100% paperless KYC verification. Open your investment account within minutes &amp; start an SIP in mutual
            funds with just Rs.100 on the very same day. Take an assessment of your appetite for risk with our Free Risk
            Profile Assessment. Explore and invest in the
            <a class="text-[#00baf2]" href="https://www.paytmmoney.com/mutual-funds/benefits">best mutual funds</a> rated
            by leading research
            agencies and achieve your personal and financial goals.
          </p>
          <p class="text-[#707070] py-[12px]">At Paytm Money, you can manage your SIPs, request portfolio-related
            statements and view the latest portfolio
            updates. Enjoy the
            <a class="text-[#00baf2]" href="https://www.paytmmoney.com/mutual-funds/benefits/">Mutual Fund benefits </a>of
            absolutely secure
            investments on the Paytm Money platform with convenient payment options like Net Banking, UPI and auto-Pay
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Money Bank Transfer Made Instant &amp; Easy With Paytm</h2>
          <p class="text-[#707070] py-[12px]">Transferring money directly to the bank from Paytm is instant and free of
            cost using Paytm app. Yes, any
            Paytm user can make a
            <a class="text-[#00baf2]" href="https://paytm.com/offer/bank-transfer/"> bank transfer</a> anytime and
            anywhere in less than a
            minute. You can link any bank account using Paytm’s UPI services and no KYC is needed. Moreover, you also get
            a Cashback of Rs. 50 on your first bank transfer with Paytm. To make money transfer process fast &amp;
            trouble-free, you can link your account with Paytm in just a few simple steps. Next, you just have to enter
            the details of the account holder, precisely IFSC code and account number &amp; you are all set to make a bank
            transfer at 0% charges.
          </p>
          <h2 class="font-semibold text-[#505050] pb-1">Events, Movies and Endless Entertainment- Live, Laugh, Enjoy with
            Paytm.com</h2>
          <p class="text-[#707070] py-[12px]">Relive the moment and revive your daily routine with an amazing experience
            at an incredible amusement park.
            Book tickets for theme parks &amp; water parks in seconds at Paytm.com and get ready to make your day an
            adventurous one. Enjoy the hottest buzz in the town, do not miss out the latest shows and events of your
            favourite artists, be it music concert or a carnival, book your tickets online at our portal and catch the
            beats without any hassle. Our entertainment section enables you to book tickets online for Movies and Events
            at the matter of a few clicks and escape from your busy schedule.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">Movie Ticket Booking</span>- Find movie showtimes, movie theatres
            to book your movie tickets online and
            get movie ticket offers only on Paytm.com
          </p>
          <p class="text-[#707070] py-[12px]">Paytm’s
            <a class="text-[#00baf2]" href="https://paytm.com/care/ticket">24x7
              Help is always at your service to assist you in case of any difficulties.
            </a>
          </p><a class="text-[#00baf2]" href="https://paytm.com/care/ticket">
            <h2 class="font-semibold text-[#505050] pb-1">Investments made Simple, Transparent and Accessible with Paytm
              Money</h2>
          </a>
          <p class="text-[#707070] py-[12px]"><a class="text-[#00baf2]" href="https://paytm.com/care/ticket">
              <span class="text-[#505050] font-semibold">Presenting Paytm Money</span> - India's Most Sincere Wealth
              Adviser. You can now begin your
            </a><a class="text-[#00baf2]" href="https://www.paytmmoney.com/">Investment</a> journey on the Paytm Money App
            with 100% paperless
            KYC verification. Open your investment account within minutes &amp; start investing. Take an assessment of
            your appetite for risk with our Free Risk Profile Assessment.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">
              <a class="text-[#00baf2]" href="https://www.paytmmoney.com/mutual-funds">Mutual Funds</a>
            </span> - Our first offering to enable users to invest in direct mutual funds. In this, you get to save on
            commissions &amp; earn up to 1% higher returns than regular funds. Easy SIP management and a fully digital KYC
            process would make your investing experience more rewarding.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">
              <a class="text-[#00baf2]" href="https://www.paytmmoney.com/nps-national-pension-scheme">National Pension
                System (NPS)</a>
            </span> - This latest addition to our tax-saving product basket helps you to earn market-linked returns and
            accumulate a higher corpus for a comfortable retirement. Additionally, you get to claim an extra tax deduction
            of up to Rs 50,000 over and above Section 80C benefit of Rs 1,50,000 and save Rs 62,400 in taxes annually.
          </p>
          <p class="text-[#707070] py-[12px]">
            <span class="text-[#505050] font-semibold">
              <a class="text-[#00baf2]" href="https://www.paytmmoney.com/stocks"> Stocks</a>
            </span> - Stocks are now live on Paytm Money. With a 100% paperless account opening and a fully digital KYC
            process, you can become investment-ready within 24 hours. Moreover, you can enjoy both intraday trading in
            stocks &amp; Zero Brokerage on delivery trading for life! Also, you can set price alerts &amp; create multiple
            watchlists to track real-time price changes of up to 50 stocks.
          </p>
          <div
            class="w-full bg-[#f5f7fa] h-4 relative flex flex-col justify-center items-center transition-all duration-300 overflow-hidden"
            :class="{ 'h-fit': openFaq, 'h-0': !openFaq }">
            <div
              class="w-full bg-[#f5f7fa] h-4 absolute flex justify-between text-xs items-center top-0 left-0 z-30 cursor-pointer"
              @click="openFaq = !openFaq">
              <h1 class="text-xs font-semibold py-[16px]">Frequently Asked Questions</h1>
              <Icon name="tdesign:plus" class="transition-all duration-300 text-sm"
                :class="{ 'rotate-[225deg]': openFaq }" />
            </div>
            <div class="w-full top-0 p-0 transition-all duration-300 text-xs text-[#505050]"
              :class="{ 'pt-5': openFaq, 'p-0': !openFaq }">
              <h2 class="mt-[10px] font-semibold">What is Paytm?</h2>
              <p class="my-[12px]">Paytm stands for Pay through mobile and it is India’s largest mobile payments and
                commerce platform. It
                lets you transfer money instantly to anyone at zero cost using the Paytm Wallet. You can make cashless
                transactions at several places like taxi and autos, petrol pumps, grocery shops, restaurants, coffee
                shops, multiplexes, and many more. You can also use Paytm to pay for online recharges, utility bill
                payments, book movie or travel tickets among other things on the Paytm app or website.</p>
              <h2 class="mt-[10px] font-semibold">How to create Paytm account?</h2>
              <p class="my-[12px]">1. Open your Paytm app
                <br>2. Tap on ‘Create A New Account’
                <br>3. Enter your mobile that you want to use for Paytm, email address and a password
                <br>4. Tap on ‘Create a New Account’
                <br>5. Enter the OTP that you will receive on your mobile number and click on ‘Submit’
                <br>6. Enter your First Name, Last Name and DOB
                <br>7. Click on ‘Create Account’
                <br>8. Your account has been created
              </p>
              <h2 class="mt-[10px] font-semibold">How to use Paytm?</h2>
              <p class="my-[12px]">You can use Paytm for many different things such as online recharge, shopping, pay
                fees, bills and a
                lot more thing. You will need to at least one of your bank account to your Paytm account and then you
                can enjoy India’s fastest online transactions and payment service. </p>
              <h2 class="mt-[10px] font-semibold">How to transfer money back from Paytm to bank account?</h2>
              <p class="my-[12px]">Follow the steps to transfer money from Paytm wallet to a bank account-</p>
              <p>1. Open your ‘Passbook in your Paytm app
                <br>2. Click on ‘Send Money to Bank’
                <br>3. Enter the transaction amount and account details
                <br>4. Click on ‘Proceed’
                <br>5. Your transaction is complete.
              </p>
              <p class="my-[12px]">Note that Paytm charges you 4% of the transaction when you transfer money from your
                Paytm wallet to a
                bank account. </p>
              <h2 class="mt-[10px] font-semibold">How to do KYC in Paytm?</h2>
              <p class="my-[12px]">To do your KYC in Paytm, you need to log in to your account on Paytm app and follow
                these steps-</p>
              <p class="mb-[12px]">1. Go to your ‘My Profile Settings’ section in Paytm app.
                <br>2. Tap on ‘Complete your KYC’
                <br>3. Select your state and district
                <br>4. You will see a list of KYC centres as per the details you have filled. Go to the nearby KYC store
                to complete your KYC. You will have to carry the required documents such as Aadhar card, Voter ID card,
                PAN card etc.
              </p>
              <h2 class="mt-[10px] font-semibold">How to get free Paytm cash back?</h2>
              <p class="my-[12px]">You can get free Paytm cash back by applying promo codes while you are proceeding your
                transactions.
                Tap on ‘Cashback’ on the top right corner of your Paytm app to find daily promo codes and offers. You
                can get additional cash back by purchasing a gift voucher on Paytm.</p>
              <h2 class="mt-[10px] font-semibold">How to add beneficiary in Paytm?</h2>
              <p class="my-[12px]">1. Go to ‘My Payment Settings’ on Paytm app.
                <br>2. Tap on ‘Manage Beneficiaries’
                <br>3. Tap on ‘Add New Beneficiary’
                <br>4. Enter account details or wallet number of the beneficiary.
                <br>5. Tap on ‘Add Beneficiary’
                <br>6. Enter OTP received on your number
                <br>7. Beneficiary is added succesfully
              </p>
              <h2 class="mt-[10px] font-semibold">How to add money in Paytm wallet?</h2>
              <p class="my-[12px]">To add money in your Paytm wallet follow these simple steps-</p>
              <p class="my-12px">1. Go to your ‘Passbook’
                <br>2. Tap on ‘Paytm Wallet’
                <br>3. Tap on ‘Add money to Paytm Wallet’
                <br>4. Enter the amount you want to add in your wallet and click on ‘Add Money’
                <br>5. Select your mode of the transaction- bank account, debit card, credit card, net banking or BHIM
                UPI
                <br>6. Enter account/card details and tap on ‘Pay Securely’
                <br>7. Enter OTP that you will receive on your mobile number
                <br>8. Money is added in your wallet
              </p>
              <h2 class="mt-[10px] font-semibold">How to pay through Paytm?</h2>
              <p class="my-[12px]">1. Tap on ‘Pay’ on Paytm app
                <br>2. Scan the QR code or enter the number of the beneficiary that you want to pay
                <br>3. Enter the amount
                <br>4. Pay using your Paytm wallet or add money to your Paytm wallet from your bank account if the
                wallet has insufficient funds
                <br>5. The money is paid to the beneficiary
              </p>
              <h2 class="mt-[10px] font-semibold">How to use Paytm in Hindi?</h2>
              <p class="my-[12px]">1. Download Paytm App from here
                <br>2. Tap on the top left corner button on your Paytm app
                <br>3. Tap on ‘Choose Language’
                <br>4. Select ‘Hindi’ as the language and tap on ‘Continue’
                <br>5. You can use your Paytm app in Hindi now
              </p>
              <h2 class="mt-[10px] font-semibold">How to contact Paytm customer care executive? </h2>
              <p class="my-[12px]">You can get in touch with the customer care executive by calling at one of the
                following Paytm customer
                care numbers-</p>
              <p class="my-[12px]">1. Bank, Wallet and Payments- 0120-4456-456
                <br>2. Movies and Events Tickets- 0120-4728-728
                <br>3. Paytm Mall Shopping Orders- 0120-4606060
                <br>4. Paytm Travel Tickets and Forex- 0120-4880-880
              </p>
              <h2 class="mt-[10px] font-semibold">How to pay electricity bill by Paytm?</h2>
              <p class="my-[12px]">1. Go to electricity bill payment page on Paytm website or Paytm app
                <br>2. Select your state
                <br>3. Select your board
                <br>4. Enter your consumer number
                <br>5. Pay your bill through debit card, credit card, net banking or Paytm wallet
              </p>
              <h2 class="mt-[10px] font-semibold"> How to reset Paytm password?</h2>
              <p class="my-[12px]">1. Tap on ‘My Security Settings’ on your Paytm app
                <br>2. Select ‘Change Password’
                <br>3. Enter your current password
                <br>4. Enter a new password and retype your new password in the box belowTap on ‘Save’
                <br>5. Your password has been changed
              </p>
            </div>
          </div>
          <div class="flex justify-center items-center flex-col">
            <div class="flex flex-col gap-3 md:flex-row items-center overflow-visible p-3 mt-[16px]">
              <div
                class="flex p-3 justify-center items-center w-[350px] sm:w-full max-w-[500px] bg-white rounded-2xl shadow-md">
                <img class="w-14" src="https://pwebassets.paytm.com/commonwebassets/paytmweb/footer/images/help.svg"
                  alt="">
                <p class="text-xs text-[#707070]"><span class="text-[#505050] font-bold">24X7 Help</span> If we fall short
                  of your expectations in any way, let us know.</p>
              </div>
              <div
                class="flex p-3 justify-center items-center w-[350px] sm:w-full max-w-[500px] bg-white rounded-2xl shadow-md">
                <img class="w-14" src="https://pwebassets.paytm.com/commonwebassets/paytmweb/footer/images/assurance.svg"
                  alt="">
                <p class="text-xs text-[#707070]"><span class="text-[#505050] font-bold">100% Assurance</span> If you face
                  any issue, your money is immediately refunded. Sit back shop on.</p>
              </div>
              <div
                class="flex p-3 justify-center items-center w-[350px] sm:w-full max-w-[500px] bg-white rounded-2xl shadow-md">
                <img class="w-14" src="https://pwebassets.paytm.com/commonwebassets/paytmweb/footer/images/trust.svg"
                  alt="">
                <p class="text-xs text-[#707070]"><span class="text-[#505050] font-bold">Paytm Trust </span> Your money is
                  yours. All refunds come with no question asked guarantee.</p>
              </div>
            </div>
            <div class="w-full">
              <div class="w-full mb-[16px] p-[30px] grid grid-cols-2 gap-6 md:grid-cols-8">
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">About Us</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">24x7 Help</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">Partner <br> with us</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">Grivance <br> policy</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">Blog</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">Bug Bounty</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">Privacy</nuxt-link>
                </div>
                <div class="w-full text-xs text-center overflow-hidden">
                  <nuxt-link class="hover:text-[#000] hover:font-semibold transition-all duration-300 hover:text-nowrap hover:text-[14px]" to="/">Terms & <br> Conditions</nuxt-link>
                </div>
              </div>
              <div class="w-full p-[30px] flex justify-center gap-8">
                <div class="w-[300px] sm:w-full border-2 border-[#85eefc] py-[12px] px-[18px] rounded-xl hover:bg-[#85eefc] transition-all duration-300 cursor-pointer">
                  <p class="text-xs font-semibold text-black">Become a Seller & Earn</p>
                </div>
                <div class="w-[300px] sm:w-full border-2 border-[#85eefc] py-[12px] px-[18px] rounded-xl hover:bg-[#85eefc] transition-all duration-300 cursor-pointer">
                  <p class="text-xs font-semibold text-black">Become a Seller & Earn</p>
                </div> 
              </div>
            </div>
          </div>
        </div>
      </Acord>
      <Acord title="Investor Relations" :initialOpen="openAcord === 3" @toggle="toggleAccord(3)">
        test
      </Acord>
      <Acord title="Investor Relations" :initialOpen="openAcord === 4" @toggle="toggleAccord(4)">
        test
      </Acord>
    </div>
    <div class="w-full pt-[30px] pb-[50px] flex justify-center">
      <p class="text-[#707070] text-xs">Copyright © 2023 Paytm All rights reserved</p>
    </div>
  </div>
</template>

<script setup>
const openAcord = ref(0)
const innerAcord = ref(0)

const openFaq = ref(false)

const toggleInnerAcord = (index) => {
  if (innerAcord.value === index) {
    innerAcord.value = 0;
  } else {
    innerAcord.value = index
  }
}

const toggleAccord = (index) => {
  if (openAcord.value === index) {
    openAcord.value = 0;
  } else {
    openAcord.value = index
  }
}

</script>

