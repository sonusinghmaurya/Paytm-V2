<template>
  <div class="w-full">
    <section
      class="w-full relative pt-[40px] pb-[60px] sm:pt-[80px] flex flex-col-reverse sm:flex-row items-center xl:px-[120px] 2xl:px-[226px]">
      <div class="w-full flex justify-between items-center px-4">
        <div class="w-full p-5 flex flex-col justify-center gap-7 flex-1">
          <div class="shadow-lg w-fit">
            <img class="w-[50px] md:w-[80px]" src="/assets/images/home/paytm_app_logo.png" alt="" />
          </div>
          <div class="w-fit flex flex-col justify-start">
            <h1 class="text-[32px] text-nowrap font-bold leading-9 mt-4 md:text-[42px] md:leading-tight lg:text-[62px]">
              India's Most-loved <br />
              Payments App
            </h1>
            <p class="text-nowrap text-[14px] font-medium pt-3 mb-5 md:text-[18px] lg:text-[22px]">
              Recharge & pay bills, book flights & movie tickets, <br />
              open a savings account, invest in stocks & mutual <br />
              funds, and do a lot more
            </p>
            <nuxt-link
              class="bg-black border transition-all duration-300 border-black px-[14px] py-[10px] mt-5 shadow-sm text-[14px] text-white rounded-[35px] flex justify-center items-center gap-1 w-fit hover:bg-white hover:text-black sm:text-[16px] md:text-[20px] sm:px-[24px]"
              to="/">
              <span>Download the Paytm App</span>
              <Icon name="ic:baseline-apple" class="text-[20px]" />
              <Icon name="ion:logo-google-playstore" />
            </nuxt-link>
          </div>
        </div>
        <div
          class="absolute top-[40px] right-[-20px] translate-x-[-50%] translate-y-[-50px] w-[150px] sm:relative sm:w-96 sm:translate-x-0 sm:translate-y-0 sm:top-0 sm:right-0 p-5 flex-1 flex justify-center items-center">
          <img class="" src="/assets/images/home/home_1.png" alt="" />
        </div>
      </div>
    </section>
    <section
      class="w-full bg-[#00baf2] flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <h1 class="text-white text-[24px] font-bold sm:text-[28px] md:text-[32px] lg:text-[38px] xl:text-[42px]">
        Recharge & Pay Bills on Paytm
      </h1>
      <div class="w-full grid grid-cols-2 gap-10 sm:grid-cols-3 md:grid-cols-5 lg:grid-cols-7">
        <ColItemsHomeitem name="Recharge" type="Prepaid" device="Mobile"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/733299/1626251017535.png" />
        <ColItemsHomeitem name="Pay" type="Electricity" device="Bill"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/733308/1626251043534.png" />
        <ColItemsHomeitem name="Recharge" type="DTH" device="Connection"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/733311/1626251101045.png" />
        <ColItemsHomeitem name="Book" type="Gas" device="Cylinder"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/733307/1626251127863.png" />
        <ColItemsHomeitem name="Pay" type="Broadband &" device="Landline Bill"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/1269194/1672827522093.png" />
        <ColItemsHomeitem name="Pay" type="Education" device="Fee"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/1269198/1672828917034.png" />
        <ColItemsHomeitem name="All" type="Payment" device="Services"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/757701/1626268580682.png" />
      </div>
    </section>
    <section
      class="w-full bg-[#0f4a8a] flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <h1 class="text-white text-[24px] font-bold sm:text-[28px] md:text-[32px] lg:text-[38px] xl:text-[42px]">
        Book & Buy on Paytm.
      </h1>
      <div class="w-full grid grid-cols-2 gap-10 sm:grid-cols-3 md:grid-cols-5 lg:grid-cols-7">
        <ColItemsSecontitem name="Movie" device="Tickets"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/733295/1626259710574.png" />
        <ColItemsSecontitem name="Flight" device="Tickets"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/733296/1626259884425.png" />
        <ColItemsSecontitem name="Bus" device="Tickets"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/729996/1626260477699.png" />
        <ColItemsSecontitem name="Train" device="Tickets"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/729997/1696910636390.png" />
        <ColItemsSecontitem name="Buy" device="Insurance"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/729998/1666185237748.png" />
        <ColItemsSecontitem name="International" device="Flights"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/729999/1626259968563.png" />
        <ColItemsSecontitem name="Invest" device="In Stocks"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/730001/1626450848003.png" />
      </div>
    </section>
    <section
      class="w-full flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <h1
        class="text-black text-[24px] font-bold sm:text-[28px] md:text-[32px] lg:text-[38px] xl:text-[52px] text-nowrap mb-8">
        Paytm Payment Instruments
      </h1>
      <div
        class="sm:bg-white sm:p-[80px] rounded-3xl flex justify-between items-center w-full flex-col-reverse gap-6 sm:flex-row overflow-hidden">
        <div class="flex-1">
          <div class="flex justify-start items-center gap-4">
            <img class="w-[60px] sm:w-[100px]"
              src="https://assetscdn1.paytm.com/images/catalog/view/307185/1617861564011.png" alt="paytm">
            <p class="text-[14px] sm:text-[20px] font-bold">Paytm <br> Wallet</p>
          </div>
          <div class="mt-6">
            <h1 class="text-nowrap text-[23px] sm:text-[25px] lg:text-[42px] font-bold">The Fastest Way to<br>
              Pay In-store & Online.
            </h1>
          </div>
          <div class="py-[25px] max-w-[400px]">
            <p class="font-medium sm:text-[18px] lg:text-[20px]">
              Load up your Paytm Wallet for free and make payments in a jiffy at over 21 million stores, websites and
              apps.
            </p>
          </div>
          <nuxt-link
            class="bg-black border transition-all duration-300 border-black px-[14px] py-[10px] mt-5 shadow-sm text-[14px] text-white rounded-[35px] flex justify-center items-center gap-1 w-fit hover:bg-white hover:text-black sm:text-[16px] lg:text-[20px] sm:px-[24px] text-nowrap"
            to="/">
            <span>Download the App</span>
            <Icon name="ic:baseline-apple" class="text-[20px]" />
            <Icon name="ion:logo-google-playstore" />
          </nuxt-link>
        </div>
        <div class="flex-1 flex justify-center items-center">
          <img class="sm:m-w-[350px] sm:max-w-[350px]  lg:max-w-[500px]"
            src="https://assetscdn1.paytm.com/images/catalog/view_item/728701/1618577020961.png" alt="">
        </div>
      </div>
      <div
        class="sm:bg-white sm:p-[80px] rounded-3xl flex justify-between items-center w-full flex-col-reverse gap-6 sm:flex-row mt-24 sm:mt-8">
        <div class="flex-1">
          <div class="flex justify-start items-center gap-4">
            <img class="w-[60px] sm:w-[100px]"
              src="https://assetscdn1.paytm.com/images/catalog/view/307186/1615957674521.png" alt="paytm">
            <p class="text-[14px] sm:text-[20px] font-bold">UPI Money <br> Transfer</p>
          </div>
          <div class="mt-6">
            <h1 class="text-nowrap text-[23px] sm:text-[25px] lg:text-[42px] font-bold">Pay anyone directly<br>
              from your bank <br> account.
            </h1>
          </div>
          <div class="py-[25px] max-w-[400px]">
            <p class="font-medium sm:text-[18px] lg:text-[20px]">
              Pay anyone, everywhere. Make contactless & secure payments in-stores or online using Paytm Wallet or
              Directly from your Bank Account. Plus, send & receive money from anyone.
            </p>
          </div>
          <nuxt-link
            class="bg-black border transition-all duration-300 border-black px-[14px] py-[10px] mt-5 shadow-sm text-[14px] text-white rounded-[35px] flex justify-center items-center gap-1 w-fit hover:bg-white hover:text-black sm:text-[16px] lg:text-[20px] sm:px-[24px] text-nowrap"
            to="/">
            <span>Download the App</span>
            <Icon name="ic:baseline-apple" class="text-[20px]" />
            <Icon name="ion:logo-google-playstore" />
          </nuxt-link>
        </div>
        <div class="flex-1 flex justify-center items-center">
          <img class="sm:m-w-[350px] sm:max-w-[350px]  lg:max-w-[500px]"
            src="https://assetscdn1.paytm.com/images/catalog/view_item/728702/1626342071104.png" alt="">
        </div>
      </div>
    </section>
    <section
      class="w-full flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <div class="w-full flex justify-center items-center flex-col xl:flex-row gap-[50px]">
        <div class="flex justify-end flex-col flex-1 bg-white p-5 rounded-3xl sm:px-[40px] lg:px-[80px] pb-0">
          <div class="w-full">
            <img class="w-[140px] ml-[2px] md:w-[180px]"
              src="https://assetscdn1.paytm.com/images/catalog/view_item/853975/1640242865113.png" alt="">
          </div>
          <div class="w-full">
            <h1 class="text-[28px] font-bold pt-[28px] md:text-[35px] xl:text-[52px]">
              Unlimited Cashback <br>
              Every time
            </h1>
            <p class="text-[12px] font-semibold mt-[20px] mb-[8px] md:text-[20px]">
              Paytm HDFC Bank Select Credit Card. <br> A card with assured Cashback and incredible offers.
            </p>
            <p class="text-[11px] text-[#75767f] md:text-[14px] lg:text-[20px]">
              *Paytm Payments Bank does not provide any loan or credit <br> card on the Paytm App.
              <nuxt-link class="text-[#00baf2]" to="/">
                Know more
              </nuxt-link>
            </p>
            <div class="flex justify-center items-center">
              <img class="w-[300px] sm:w-[400px] md:w-[500px] mt-8"
                src="https://assetscdn1.paytm.com/images/catalog/view_item/853975/1640241561388.png" alt="">
            </div>
          </div>
        </div>
        <div class="flex justify-end flex-col flex-1 bg-white p-5 rounded-3xl sm:px-[40px] lg:px-[80px] pb-0">
          <div class="w-full mt-[52px]">
            <img class="w-[140px] ml-[2px] md:w-[180px]"
              src="https://assetscdn1.paytm.com/images/catalog/view_item/853976/1640242163727.png" alt="">
          </div>
          <div class="w-full">
            <h1 class="text-[28px] font-bold pt-[28px] md:text-[35px] xl:text-[52px]">
              India’s Most <br>
              Sincere Credit Card
            </h1>
            <p class=" text-[12px] font-semibold mt-[20px] mb-[8px] md:text-[20px]">
              Paytm SBI Card SELECT - With Intelligent <br> Features & Great Rewards that Never Expire
            </p>
            <p class=" text-[11px] text-[#75767f] md:text-[14px] lg:text-[20px]">
              *Paytm Payments Bank does not provide any loan or credit <br> card on the Paytm App.
              <nuxt-link class="text-[#00baf2]" to="/">
                Know more
              </nuxt-link>
            </p>
            <div class="flex justify-center items-center">
              <img class="w-[300px] sm:w-[400px] md:w-[500px] mt-8"
                src="https://assetscdn1.paytm.com/images/catalog/view_item/853976/1626079147084.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="w-full bg-white flex justify-center items-center">
      <div
        class="w-full flex items-start px-[20px] py-[80px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
        <h1
          class="p-5 text-black text-[20px] font-bold sm:text-[28px] md:text-[32px] lg:text-[38px] xl:text-[52px] text-nowrap mb-8">
          Financial Services by Paytm</h1>
        <div class="w-full flex justify-between">
          <div class="max-w-[550px] p-5 flex-1">
            <div class="pb-[12px]">
              <img class="w-[200px]" src="https://assetscdn1.paytm.com/images/catalog/view/307193/1617696576778.png"
                alt="logo">
            </div>
            <div class="w-full">
              <h2 class="font-bold text-[28px] mt-[24px] md:text-[35px] xl:text-[52px]">India's most sincere <br> bank.
              </h2>
              <h5 class="text-[14px] text-black font-medium pt-[12px] mb-[24px] md:text-[20px]">
                Paytm Payments Bank offers secure, transparent and risk-free banking at your fingertips. With instant
                account opening, virtual debit card and zero balance requirements, experience the future of banking today.
              </h5>
              <nuxt-link to="/"
                class="group flex justify-center items-center transition-all duration-300 text-white bg-[#002970] w-fit px-[25px] py-[10px] rounded-[25px] hover:bg-[#00baf2] lg:text-[20px]">
                <span>Learn More</span>
                <div class="relative ml-1 flex justify-center items-center">
                  <span
                    class="absolute w-0 h-[2px] duration-300 bg-white top-[50%] rounded-md left-[55%] translate-x-[-50%] translate-y-[-50%] group-hover:w-3"></span>
                  <Icon name="fluent:ios-arrow-right-24-filled"
                    class="transition-all duration-300 group-hover:translate-x-[2px]" />
                </div>
              </nuxt-link>
            </div>
          </div>
          <div class="max-w-[550px] p-5 flex-1 hidden sm:flex">
            <img src="https://assetscdn1.paytm.com/images/catalog/view_item/728826/1626076427497.png" alt="">
          </div>
        </div>
      </div>
    </section>
    <section class="w-full p-2  flex flex-colitems-center justify-center relative overflow-hidden">
      <div
        class="absolute bottom-0 left-0 w-full h-[300px] sm:h-[400px] md:h-[550px] bg-[url('https://pwebassets.paytm.com/commonwebassets/commonweb/images/home/gray-spike.png')] bg-cover bg-no-repeat">
      </div>
      <div
        class="w-full flex items-center px-[50px] py-[50px] z-0 flex-col sm:flex-row gap-10 sm:justify-between xl:px-[120px] 2xl:px-[226px]">
        <div class="flex justify-center items-center">
          <img class="w-full sm:w-[400px] md:w-[500px] xl:max-w-[650px] aspect-auto"
            src="https://assetscdn1.paytm.com/images/catalog/view_item/788781/1626077377376.png" alt="">
        </div>
        <div class="flex-1 max-w-[500px] w-full">
          <div class="">
            <img class="w-[120px] hidden sm:flex"
              src="https://assetscdn1.paytm.com/images/catalog/view/308774/1617696247991.png" alt="">
          </div>
          <h1 class="font-bold text-nowrap text-[23px] mt-[24px] md:text-[26px] xl:text-[52px]">
            Build Long-term <br>
            Wealth & Achieve <br>
            your Goals
          </h1>
          <h5 class="text-[14px] text-black font-medium pt-[12px] mb-[24px] md:text-[20px]">
            Investing on Paytm Money is transparent, low-cost and commission-free. Buy stocks & mutual funds that can help
            you create wealth & realise your dreams.
          </h5>
          <nuxt-link to="/"
            class="group flex justify-center items-center transition-all duration-300 text-white bg-[#002970] w-fit px-[25px] py-[10px] rounded-[25px] hover:bg-[#00baf2] lg:text-[20px]">
            <span>Learn More</span>
            <div class="relative ml-1 flex justify-center items-center">
              <span
                class="absolute w-0 h-[2px] duration-300 bg-white top-[50%] rounded-md left-[55%] translate-x-[-50%] translate-y-[-50%] group-hover:w-3"></span>
              <Icon name="fluent:ios-arrow-right-24-filled"
                class="transition-all duration-300 group-hover:translate-x-[2px]" />
            </div>
          </nuxt-link>
        </div>
      </div>
    </section>
    <section
      class="w-full bg-white flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <div class="w-full flex justify-between">
        <div class="max-w-[550px] p-5 flex-1">
          <div class="pb-[12px]">
            <img class="w-[200px]" src="https://assetscdn1.paytm.com/images/catalog/view/308775/1653901470333.jpeg"
              alt="logo">
          </div>
          <div class="w-full">
            <h2 class="font-bold text-[28px] mt-[24px] md:text-[35px] xl:text-[52px]">Insurance made easy.
            </h2>
            <h5 class="text-[14px] text-black font-medium pt-[12px] mb-[24px] md:text-[20px]">
              Buying insurance does not have to be tedious, time-consuming & confusing. Paytm Insurance removes the worry
              of getting insured by making it simple, convenient & easy-to-understand.
            </h5>
            <nuxt-link to="/"
              class="group flex justify-center items-center transition-all duration-300 text-white bg-[#002970] w-fit px-[25px] py-[10px] rounded-[25px] hover:bg-[#00baf2] lg:text-[20px]">
              <span>Learn More</span>
              <div class="relative ml-1 flex justify-center items-center">
                <span
                  class="absolute w-0 h-[2px] duration-300 bg-white top-[50%] rounded-md left-[55%] translate-x-[-50%] translate-y-[-50%] group-hover:w-3"></span>
                <Icon name="fluent:ios-arrow-right-24-filled"
                  class="transition-all duration-300 group-hover:translate-x-[2px]" />
              </div>
            </nuxt-link>
          </div>
        </div>
        <div class="max-w-[550px] p-5 flex-1 hidden sm:flex">
          <img src="https://assetscdn1.paytm.com/images/catalog/view_item/788790/1653913927257.png" alt="">
        </div>
      </div>
    </section>
    <section
      class="w-full flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <div class="w-full flex justify-between flex-col md:flex-row">
        <div class="ww-full] max-w-[550px] p-5 flex-1 flex justify-center items-center">
          <img class="w-[350px] md:w-[500px]"
            src="https://assetscdn1.paytm.com/images/catalog/view_item/850765/1655987252365.png" alt="">
        </div>
        <div class="max-w-[550px] p-5 flex-1">
          <div class="pb-[12px]">
            <img class="w-[200px]" src="https://assetscdn1.paytm.com/images/catalog/view/308777/1617695287770.png"
              alt="logo">
          </div>
          <div class="w-full">
            <h2 class="font-bold text-nowrap text-[28px] mt-[24px] md:text-[35px] xl:text-[52px]">Get a Personal Loan in
              <br>2 Minutes.
            </h2>
            <h5 class="text-[14px] text-black font-medium pt-[12px] mb-[24px] md:text-[18px]">
              Paytm offers India's quickest multi-purpose, hassle-free loan. It is 100% digital, transparent and
              paperless.
            </h5>
            <nuxt-link to="/"
              class="group flex justify-center items-center transition-all duration-300 text-white bg-[#002970] w-fit px-[25px] py-[10px] rounded-[25px] hover:bg-[#00baf2] lg:text-[20px]">
              <span>Learn More</span>
              <div class="relative ml-1 flex justify-center items-center">
                <span
                  class="absolute w-0 h-[2px] duration-300 bg-white top-[50%] rounded-md left-[55%] translate-x-[-50%] translate-y-[-50%] group-hover:w-3"></span>
                <Icon name="fluent:ios-arrow-right-24-filled"
                  class="transition-all duration-300 group-hover:translate-x-[2px]" />
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </section>
    <section
      class="w-full bg-white flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <h1 class="text-[24px] font-bold sm:text-[26px] md:text-[28px] lg:text-[42px]">Business Services by Paytm</h1>
      <div class="w-full h-full bg-[#f5f7fa] rounded-2xl mt-9 flex justify-between
      items-center flex-col gap-10 md:flex-row py-[50px] pl-[10px] sm:pl-[50px]">
        <div class="w-full flex-1">
          <h1 class="text-[22px] font-semibold sm:text-[26px] md:text-[28px] lg:text-[58px]">Accept payments <br>
            online with ease</h1>
          <p class="py-[20px] sm:py-[40px] text-[14px] sm:text-[18px] lg:text-[20px]">
            Grow your business with the payment gateway that <br> powers India’s largest brands and even the Paytm App
          </p>
          <nuxt-link to="/"
            class="group flex justify-center items-center transition-all duration-300 text-white bg-[#002970] w-fit px-[25px] py-[10px] rounded-[25px] hover:bg-[#00baf2] lg:text-[20px]">
            <span>Learn More</span>
            <div class="relative ml-1 flex justify-center items-center">
              <span
                class="absolute w-0 h-[2px] duration-300 bg-white top-[50%] rounded-md left-[55%] translate-x-[-50%] translate-y-[-50%] group-hover:w-3"></span>
              <Icon name="fluent:ios-arrow-right-24-filled"
                class="transition-all duration-300 group-hover:translate-x-[2px]" />
            </div>
          </nuxt-link>
        </div>
        <div class="w-full flex-1 flex items-center justify-end">
          <img class=" w-[350px] lg:w-[550px]"
            src="https://assetscdn1.paytm.com/images/catalog/view_item/853877/1697527245473.png" alt="">
        </div>
      </div>
      <div class="w-full h-full bg-[#f5f7fa] rounded-2xl mt-9 flex justify-between
      items-center flex-col gap-10 md:flex-row py-[50px] pl-[10px] sm:pl-[50px]">
        <div class="w-full flex-1">
          <h1 class="text-[22px] font-semibold sm:text-[26px] md:text-[28px] lg:text-[58px]">In-shop payments <br>
            online with ease</h1>
          <p class="py-[20px] sm:py-[40px] text-[14px] sm:text-[18px] lg:text-[20px]">
            Millions of small & big businesses use Paytm to accept <br> payments anywhere any time with a wide range of
            <br> solutions for all kind of merchants
          </p>
          <nuxt-link to="/"
            class="group flex justify-center items-center transition-all duration-300 text-white bg-[#002970] w-fit px-[25px] py-[10px] rounded-[25px] hover:bg-[#00baf2] lg:text-[20px]">
            <span>Learn More</span>
            <div class="relative ml-1 flex justify-center items-center">
              <span
                class="absolute w-0 h-[2px] duration-300 bg-white top-[50%] rounded-md left-[55%] translate-x-[-50%] translate-y-[-50%] group-hover:w-3"></span>
              <Icon name="fluent:ios-arrow-right-24-filled"
                class="transition-all duration-300 group-hover:translate-x-[2px]" />
            </div>
          </nuxt-link>
        </div>
        <div class="w-full flex-1 flex items-center justify-end">
          <img class=" w-[350px] lg:w-[550px]"
            src="https://assetscdn1.paytm.com/images/catalog/view_item/853880/1656675942486.png" alt="">
        </div>
      </div>
    </section>
    <section
      class="w-full bg-white flex items-start px-[20px] py-[50px] flex-col gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <h1 class="text-[24px] font-bold sm:text-[26px] md:text-[28px] lg:text-[42px]">Business Tools to help <br> your
        business growth</h1>
      <div class="w-full grid grid-cols-1 gap-16 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4">
        <CardItemsCardItemhome headtext1="POS Billing" headtext2="Software"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/854033/1626081565192.png"
          para="Say Hello to Smart Retail Business Management" />
        <CardItemsCardItemhome headtext1="Paytm for" headtext2="Business App"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/854035/1626081071077.png"
          para="Everything you need to manage your business on your phone" />
        <CardItemsCardItemhome headtext1="Advertise on" headtext2="Paytm"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/854036/1656568216166.png"
          para="Grow your business by advertising on India’s largest mobile business" />
        <CardItemsCardItemhome headtext1="Business" headtext2="Khata"
          image="https://assetscdn1.paytm.com/images/catalog/view_item/854038/1626081814411.png"
          para="Managing Khata made easy" />
      </div>
    </section>
    <section
      class="w-full bg-white flex items-start px-[20px] py-[50px] gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <div class="flex flex-col md:flex-row">
        <div class="w-[200px] h-[240px] mr-[40px]">
          <div class="mb-7">
            <img class="w-[160px]" src="https://assetscdn1.paytm.com/images/catalog/view/307196/1626420555412.png" alt="">
          </div>
          <div class="flex flex-col gap-1">
            <p class="text-[15px] mt-[15px]">
              Get started on a wealth creation journey with Zero brokerage fee & no hidden charges.
            </p>
            <nuxt-link class="capitalize text-[15px] mt-2 text-[#00baf2]" to="/">Learn more</nuxt-link>
          </div>
        </div>
        <ul class="flex items-center flex-wrap  gap-5">
          <li class="list-none" v-for="(item, index) in items" :key="index">
            <CardItemsPaytmmoney :image="item.image" :text="item.text" />
          </li>
        </ul>
      </div>
    </section>
    <section
      class="w-full bg-white flex items-start px-[20px] py-[50px] gap-3 sm:gap-5 lg:gap-6 xl:px-[120px] 2xl:px-[226px]">
      <div class="flex flex-col md:flex-row">
        <div class="w-[200px] h-[240px] mr-[40px]">
          <div class="mb-7">
            <img class="w-[160px]" src="https://assetscdn1.paytm.com/images/catalog/view/307197/1626419838546.png" alt="">
          </div>
          <div class="flex flex-col gap-1">
            <p class="text-[15px] mt-[15px]">
              Best travel solutions with quick ticket bookings, great offers and easy refunds
            </p>
            <nuxt-link class="capitalize text-[15px] mt-2 text-[#00baf2]" to="/">Learn more</nuxt-link>
          </div>
        </div>
        <ul class="flex items-center flex-wrap  gap-5">
          <li class="list-none" v-for="(item, index) in nextItems" :key="index">
            <CardItemsPaytmtravel :image="item.image" :text="item.text" />
          </li>
        </ul>
      </div>
    </section>
    <Footer />
  </div>
</template>


<script setup>

const items = [
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/728894/1618576143299.png',
    text: 'Invest in Stocks'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/728895/1618575899205.png',
    text: 'Apply for IPO'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/800760/1618831809222.png',
    text: 'Invest in ETFs'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/728896/1618575990183.png',
    text: 'Buy Gold'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/728899/1618576408440.png',
    text: 'Invest in Mutual Funds'
  },
];

const nextItems = [
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/863734/1627552693557.png',
    text: 'Flat 14% Cashback With Code WELCOMEFLIGHT'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/864144/1627566096011.png',
    text: '100% Refund With Paytms Canncellation Protect'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/864145/1627566172335.png',
    text: 'Flat 10% Cashback With Code HAPPYBUS'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/864151/1627567062180.png',
    text: 'Sanitised Bus Option With TravelSafe+'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/864152/1696910826276.png',
    text: 'Hassle Free Train Ticket Bookings'
  },
  {
    image: 'https://assetscdn1.paytm.com/images/catalog/view_item/864153/1627566396231.png',
    text: 'PNR Status Check in Few Simple Clicks'
  }

]

</script>
