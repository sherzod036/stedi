<template>
  <section class="contacts">
    <div class="container">
      <div
        class="row"
        data-aos="fade-up"
        data-aos-duration="1500"
        data-aos-delay="0"
      >
        <div class="col-sm-6 col-md-6 col-lg-6 col-xl-4">
          <div class="contact">
            <span class="contact__title">{{ $t('address') }}:</span>
            <a href="#" class="contact__link" v-html="$t('main_location')"></a>
          </div>
        </div>
        <div class="col-sm-6 col-md-6 col-lg-6 col-xl-3">
          <div class="contact">
            <span class="contact__title">{{ $t('contactsTitle') }}:</span>
            <a href="tel:+998781290029" class="contact__link">(78) 129-00-29</a
            ><br />
            <a href="mailto:info@stedi.uz" class="contact__link">
              info@stedi.uz
            </a>
          </div>
        </div>
        <div class="col-sm-6 col-md-6 col-lg-6 col-xl-3">
          <div class="contact">
            <span class="contact__title" v-html="$t('subscribe')"></span>
            <a href="#" class="contact__link">Telegram</a><br />
            <a href="#" class="contact__link">Instagram</a><br />
            <a href="#" class="contact__link">Facebook</a><br />
          </div>
        </div>
        <div class="col-sm-6 col-md-6 col-lg-6 col-xl-2">
          <div class="contact">
            <span class="contact__icon">
              <svg
                width="132"
                height="184"
                viewBox="0 0 132 184"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  opacity="0.5"
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M0.789625 40.4262C0.765313 39.9541 0.755147 39.4814 0.760804 39.133C0.486567 25.9817 11.405 16.34 22.276 10.7004C35.3221 3.93282 51.1564 1.06609 65.5969 0.835969C80.0368 0.605276 95.8072 2.9671 108.692 9.32083C118.907 14.3566 129.242 23.0935 129.497 35.3617C129.519 35.831 129.528 36.3014 129.524 36.6469L131.76 144.324C131.781 144.787 131.792 145.251 131.787 145.715C131.628 158.754 121.144 168.292 110.273 173.932C97.2259 180.699 81.3911 183.566 66.9517 183.797C52.5118 184.027 36.7403 181.665 23.8558 175.312C13.2178 170.067 2.8631 160.856 3.02594 148.069L0.789625 40.4262ZM19.45 65.347L21.1547 147.334L21.1525 147.489C21.0807 152.575 28.3142 157.071 32.2394 159.008C42.5308 164.081 55.6544 165.853 67.175 165.669C78.694 165.485 91.8679 163.293 102.288 157.889C106.27 155.823 113.599 151.096 113.661 146.004C113.663 145.895 113.658 145.783 113.653 145.675L113.645 145.441L111.927 62.8659C111.298 63.2543 110.661 63.6292 110.019 63.9922C85.4961 77.848 46.1852 78.5842 21.5935 66.4592C20.8726 66.1035 20.1573 65.7331 19.4505 65.3464L19.45 65.347ZM111.394 37.2728L111.381 36.6689C111.009 31.8023 104.18 27.5344 100.309 25.6261C90.0184 20.5519 76.8942 18.7793 65.3747 18.9631C53.8558 19.1474 40.6818 21.3396 30.2626 26.7445C26.3063 28.7964 19.0677 33.4635 18.8913 38.5049L18.9037 39.1121C19.2769 43.9782 26.1051 48.2461 29.976 50.155C49.1316 59.5999 82.3257 59.0673 101.44 48.2682C105.048 46.2298 111.231 41.8969 111.393 37.2728L111.394 37.2728Z"
                  fill="#EC1C2C"
                />
              </svg>
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
