<template>
  <div class="mega-menu">
    <header>
			<div @click="toggleNav('mobile');" class="hamburger">
				<span>
					<svg height="32px" id="Layer_1" style="enable-background:new 0 0 32 32;" version="1.1" viewBox="0 0 32 32" width="32px" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M4,10h24c1.104,0,2-0.896,2-2s-0.896-2-2-2H4C2.896,6,2,6.896,2,8S2.896,10,4,10z M28,14H4c-1.104,0-2,0.896-2,2  s0.896,2,2,2h24c1.104,0,2-0.896,2-2S29.104,14,28,14z M28,22H4c-1.104,0-2,0.896-2,2s0.896,2,2,2h24c1.104,0,2-0.896,2-2  S29.104,22,28,22z"/></svg>
				</span>
			</div>
      <nav>
        <ul>
          <li @click="toggleNav('Technologies');">
						Technologies
					</li>
          <li>Case Studies</li>
          <li>Partners</li>
          <li>Plans</li>
          <li>Resources</li>
          <li>Company</li>
        </ul>

				<button>
					Contact Sales
				</button>
      </nav>
			<transition name="fade">
				<div v-if="navState" class="drop-down-container">
					<div class="header-mobile">

						<div class="flex-center">
							<span v-if="selectedMenu" @click="toSelectNavItem();">
								<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
								<path d="M15 18L9 12L15 6" stroke="#6E8CC5" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
								</svg>
							</span>
							<h2 v-if="selectedMenu" :class="{'green-1':navTitle.color == 1,'blue':navTitle.color == 2,'orange':navTitle.color == 3,'gray':navTitle.color == 4,}">{{navTitle.title}}</h2>
						</div>

						<div class="flex-center">
							<button>
								Contact Sales
							</button>
							<span @click="toggleNav();">
								<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
								<path d="M18 6L6 18" stroke="#233C68" stroke-width="1.5" stroke-linecap="square"/>
								<path d="M6 6L18 18" stroke="#233C68" stroke-width="1.5" stroke-linecap="square"/>
								</svg>
							</span>
						</div>
					</div>

					<section v-if="!selectedMenu">
						<div class="current-menu">
							<p>
								{{selectedNav}}
							</p>
						</div>
						<div class="grid-menu">
							<div @click="toSelectNavItem(1,'mIDentity Line');" class="grid-items heading green-1">
								<div class="heading-wrap">
									<span>
										<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
										<rect width="24" height="24" rx="3" fill="url(#paint0_linear)"/>
										<path d="M18.0762 9.04221C18.0762 5.70719 15.4039 2.94338 12.119 2.88112C10.474 2.85005 8.92427 3.46744 7.74974 4.62C6.57476 5.77289 5.92773 7.31222 5.92773 8.95432V12.7609C5.92773 13.2206 6.30041 13.5933 6.7601 13.5933C7.21979 13.5933 7.59247 13.2206 7.59247 12.7609V8.95432C7.59247 7.76281 8.06237 6.64554 8.91572 5.80829C9.76862 4.97137 10.8993 4.52356 12.0874 4.54564C14.4716 4.59081 16.4115 6.60803 16.4115 9.04233V13.1036C16.4115 13.5633 16.7841 13.936 17.2439 13.936C17.7037 13.936 18.0762 13.5633 18.0762 13.1036V9.04221Z" fill="white"/>
										<path d="M9.12012 16.605C9.12012 19.0058 11.0733 20.9591 13.4741 20.9591C15.8749 20.9591 17.828 19.0059 17.828 16.605V15.4598C17.828 15.0001 17.4555 14.6274 16.9957 14.6274C16.5359 14.6274 16.1633 15.0001 16.1633 15.4598V16.605C16.1633 18.0879 14.9569 19.2944 13.4741 19.2944C11.9912 19.2944 10.7849 18.088 10.7849 16.605V15.2324C10.7849 14.7727 10.4122 14.4 9.95249 14.4C9.4928 14.4 9.12012 14.7727 9.12012 15.2324V16.605Z" fill="white"/>
										<path d="M13.8034 17.1992C14.2632 17.1992 14.6357 16.8265 14.6357 16.3668V9.00663C14.6357 7.57141 13.5368 6.39299 12.1336 6.32374C11.4048 6.28789 10.7145 6.54471 10.1869 7.0469C9.6666 7.54222 9.36816 8.23741 9.36816 8.95436V11.6942C9.36816 12.1539 9.74084 12.5266 10.2005 12.5266C10.6602 12.5266 11.0329 12.1539 11.0329 11.6942V8.95436C11.0329 8.68723 11.1401 8.43796 11.3348 8.25273C11.529 8.06783 11.7825 7.97327 12.0517 7.98648C12.5586 8.01145 12.971 8.46914 12.971 9.00663V16.3668C12.971 16.8265 13.3436 17.1992 13.8034 17.1992Z" fill="white"/>
										<path d="M5.92773 18.9322V16.1924C5.92773 15.7327 6.30041 15.36 6.7601 15.36C7.21979 15.36 7.59247 15.7327 7.59247 16.1924V18.9322C7.59247 20.0781 5.92773 20.0781 5.92773 18.9322Z" fill="white"/>
										<defs>
										<linearGradient id="paint0_linear" x1="-5.16466" y1="-1.67853" x2="-13.5226" y2="29.8351" gradientUnits="userSpaceOnUse">
										<stop stop-color="#0DC5AB"/>
										<stop offset="1" stop-color="#2758AC"/>
										</linearGradient>
										</defs>
										</svg>
									</span>
									<label>mIDentity Line</label>
								</div>
								<div class="chevron-right">
									<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
									<path d="M10 16L14 12L10 8" stroke="#39414D" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
									</svg>
								</div>
							</div>
							<div class="menu-item">
								<div v-for="(list,index) in technology1" :key="index" class="grid-items item1-hover">
									<span>
										<img :src="list.img" alt="">
									</span>
									<div class="item1">
										<label>{{list.title}}</label>
										<small><span v-if="list.sub">{{list.sub}}</span> {{list.text}}</small>
									</div>
								</div>
							</div>
						</div>
						<div class="grid-menu">
							<div @click="toSelectNavItem(2,'mPower Line');" class="grid-items heading blue">
								<div class="heading-wrap">
									<span>
										<svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
										<rect x="0.5" width="24" height="24" rx="4" fill="#489FFF"/>
										<path d="M17.4087 10.0137C17.3608 9.91079 17.2576 9.84476 17.144 9.84476H13.681L16.0987 5.4486C16.1556 5.3586 16.1591 5.24462 16.1077 5.1514C16.0563 5.05788 15.9581 5 15.8517 5L12.1759 5C12.0652 5 11.964 5.06253 11.9144 5.16161L7.53082 12.9287C7.48551 13.019 7.49047 13.1266 7.54366 13.2128C7.59715 13.299 7.69095 13.3516 7.79236 13.3516H10.7974L8.5229 19.1286C8.46708 19.2616 8.51677 19.4159 8.63979 19.4913C8.68712 19.5202 8.73972 19.5342 8.79205 19.5342C8.87592 19.5342 8.95862 19.4983 9.01592 19.4305L17.3675 10.3254C17.4409 10.2384 17.4566 10.1168 17.4087 10.0137Z" fill="white"/>
										<defs>
										<linearGradient id="paint0_linear" x1="-4.66466" y1="-1.67853" x2="-13.0226" y2="29.8351" gradientUnits="userSpaceOnUse">
										<stop stop-color="#57BFFF"/>
										<stop offset="1" stop-color="#2555FD"/>
										</linearGradient>
										</defs>
										</svg>
									</span>
									<label for="">mPower Line</label>
								</div>
								
								<div class="chevron-right">
									<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
									<path d="M10 16L14 12L10 8" stroke="#39414D" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
									</svg>
								</div>
							</div>
							<div class="menu-item">
								<div v-for="(list,index) in technology2" :key="index" class="grid-items item2-hover">
									<span>
										<img :src="list.img" alt="">
									</span>
									<div class="item2">
										<label>{{list.title}}</label>
										<small><span v-if="list.sub">{{list.sub}}</span> {{list.text}}</small>
									</div>
								</div>
							</div>
						</div>
						<div class="grid-menu">
							<div @click="toSelectNavItem(3,'Family');" class="grid-items heading orange">	
								<div class="heading-wrap">
									<span>
										<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
										<rect width="24" height="24" rx="4" fill="#FD9D5D"/>
										<path fill-rule="evenodd" clip-rule="evenodd" d="M18.75 10C18.75 7.37665 16.6234 5.25 14 5.25H10C7.37665 5.25 5.25 7.37665 5.25 10V14C5.25 16.6234 7.37665 18.75 10 18.75H14C16.6234 18.75 18.75 16.6234 18.75 14V10ZM10 6.75H14C15.7949 6.75 17.25 8.20507 17.25 10V14C17.25 15.7949 15.7949 17.25 14 17.25H10C8.20507 17.25 6.75 15.7949 6.75 14V10C6.75 8.20507 8.20507 6.75 10 6.75Z" fill="white"/>
										<path d="M20.5 8.25H18.5C18.0858 8.25 17.75 8.58579 17.75 9C17.75 9.41421 18.0858 9.75 18.5 9.75H20.5C20.9142 9.75 21.25 9.41421 21.25 9C21.25 8.58579 20.9142 8.25 20.5 8.25Z" fill="white"/>
										<path d="M20.5 14.25H18.5C18.0858 14.25 17.75 14.5858 17.75 15C17.75 15.4142 18.0858 15.75 18.5 15.75H20.5C20.9142 15.75 21.25 15.4142 21.25 15C21.25 14.5858 20.9142 14.25 20.5 14.25Z" fill="white"/>
										<path d="M8.25 4V6C8.25 6.41421 8.58579 6.75 9 6.75C9.41421 6.75 9.75 6.41421 9.75 6V4C9.75 3.58579 9.41421 3.25 9 3.25C8.58579 3.25 8.25 3.58579 8.25 4Z" fill="white"/>
										<path d="M14.25 4V6C14.25 6.41421 14.5858 6.75 15 6.75C15.4142 6.75 15.75 6.41421 15.75 6V4C15.75 3.58579 15.4142 3.25 15 3.25C14.5858 3.25 14.25 3.58579 14.25 4Z" fill="white"/>
										<path d="M5.5 8.25H3.5C3.08579 8.25 2.75 8.58579 2.75 9C2.75 9.41421 3.08579 9.75 3.5 9.75H5.5C5.91421 9.75 6.25 9.41421 6.25 9C6.25 8.58579 5.91421 8.25 5.5 8.25Z" fill="white"/>
										<path d="M5.5 14.25H3.5C3.08579 14.25 2.75 14.5858 2.75 15C2.75 15.4142 3.08579 15.75 3.5 15.75H5.5C5.91421 15.75 6.25 15.4142 6.25 15C6.25 14.5858 5.91421 14.25 5.5 14.25Z" fill="white"/>
										<path d="M8.25 18V20C8.25 20.4142 8.58579 20.75 9 20.75C9.41421 20.75 9.75 20.4142 9.75 20V18C9.75 17.5858 9.41421 17.25 9 17.25C8.58579 17.25 8.25 17.5858 8.25 18Z" fill="white"/>
										<path d="M14.25 18V20C14.25 20.4142 14.5858 20.75 15 20.75C15.4142 20.75 15.75 20.4142 15.75 20V18C15.75 17.5858 15.4142 17.25 15 17.25C14.5858 17.25 14.25 17.5858 14.25 18Z" fill="white"/>
										<defs>
										<linearGradient id="paint0_linear" x1="-5.16466" y1="-1.67853" x2="-13.5226" y2="29.8351" gradientUnits="userSpaceOnUse">
										<stop stop-color="#FFBD52"/>
										<stop offset="1" stop-color="#F9726A"/>
										</linearGradient>
										</defs>
										</svg>
									</span>
									<label>Family</label>
								</div>
								<div class="chevron-right">
									<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
									<path d="M10 16L14 12L10 8" stroke="#39414D" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
									</svg>
								</div>
							</div>
							<div class="menu-item">
								<div v-for="(list,index) in technology3" :key="index" class="grid-items item3-hover">
									<span>
										<img :src="list.img" alt="">
									</span>
									<div class="item3">
										<label>{{list.title}}</label>
										<small><span v-if="list.sub">{{list.sub}}</span> {{list.text}}</small>
									</div>
								</div>
							</div>
						</div>
						<div class="grid-menu">
							<div @click="toSelectNavItem(4,'Technology');" class="grid-items heading gray">
								<div class="heading-wrap">
									<span>
										<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
										<rect width="24" height="24" rx="4" fill="#9FA9BA"/>
										<path fill-rule="evenodd" clip-rule="evenodd" d="M18.75 10C18.75 7.37665 16.6234 5.25 14 5.25H10C7.37665 5.25 5.25 7.37665 5.25 10V14C5.25 16.6234 7.37665 18.75 10 18.75H14C16.6234 18.75 18.75 16.6234 18.75 14V10ZM10 6.75H14C15.7949 6.75 17.25 8.20507 17.25 10V14C17.25 15.7949 15.7949 17.25 14 17.25H10C8.20507 17.25 6.75 15.7949 6.75 14V10C6.75 8.20507 8.20507 6.75 10 6.75Z" fill="white"/>
										<path d="M20.5 8.25H18.5C18.0858 8.25 17.75 8.58579 17.75 9C17.75 9.41421 18.0858 9.75 18.5 9.75H20.5C20.9142 9.75 21.25 9.41421 21.25 9C21.25 8.58579 20.9142 8.25 20.5 8.25Z" fill="white"/>
										<path d="M20.5 14.25H18.5C18.0858 14.25 17.75 14.5858 17.75 15C17.75 15.4142 18.0858 15.75 18.5 15.75H20.5C20.9142 15.75 21.25 15.4142 21.25 15C21.25 14.5858 20.9142 14.25 20.5 14.25Z" fill="white"/>
										<path d="M8.25 4V6C8.25 6.41421 8.58579 6.75 9 6.75C9.41421 6.75 9.75 6.41421 9.75 6V4C9.75 3.58579 9.41421 3.25 9 3.25C8.58579 3.25 8.25 3.58579 8.25 4Z" fill="white"/>
										<path d="M14.25 4V6C14.25 6.41421 14.5858 6.75 15 6.75C15.4142 6.75 15.75 6.41421 15.75 6V4C15.75 3.58579 15.4142 3.25 15 3.25C14.5858 3.25 14.25 3.58579 14.25 4Z" fill="white"/>
										<path d="M5.5 8.25H3.5C3.08579 8.25 2.75 8.58579 2.75 9C2.75 9.41421 3.08579 9.75 3.5 9.75H5.5C5.91421 9.75 6.25 9.41421 6.25 9C6.25 8.58579 5.91421 8.25 5.5 8.25Z" fill="white"/>
										<path d="M5.5 14.25H3.5C3.08579 14.25 2.75 14.5858 2.75 15C2.75 15.4142 3.08579 15.75 3.5 15.75H5.5C5.91421 15.75 6.25 15.4142 6.25 15C6.25 14.5858 5.91421 14.25 5.5 14.25Z" fill="white"/>
										<path d="M8.25 18V20C8.25 20.4142 8.58579 20.75 9 20.75C9.41421 20.75 9.75 20.4142 9.75 20V18C9.75 17.5858 9.41421 17.25 9 17.25C8.58579 17.25 8.25 17.5858 8.25 18Z" fill="white"/>
										<path d="M14.25 18V20C14.25 20.4142 14.5858 20.75 15 20.75C15.4142 20.75 15.75 20.4142 15.75 20V18C15.75 17.5858 15.4142 17.25 15 17.25C14.5858 17.25 14.25 17.5858 14.25 18Z" fill="white"/>
										<defs>
										<linearGradient id="paint0_linear" x1="-5.16466" y1="-1.67853" x2="-13.5226" y2="29.8351" gradientUnits="userSpaceOnUse">
										<stop stop-color="#FFBD52"/>
										<stop offset="1" stop-color="#F9726A"/>
										</linearGradient>
										</defs>
										</svg>
									</span>
									<label>Technology</label>
								</div>
								<div class="chevron-right">
									<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
									<path d="M10 16L14 12L10 8" stroke="#39414D" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
									</svg>
								</div>
							</div>
							<div class="menu-item">
								<div v-for="(list,index) in technology4" :key="index" class="grid-items item4-hover">
									<span>
										<img :src="list.img" alt="">
									</span>
									<div class="item4">
										<label>{{list.title}}</label>
										<small><span v-if="list.sub">{{list.sub}}</span> {{list.text}}</small>
									</div>
								</div>
							</div>
						</div>
					</section>
					
					<div v-if="selectedMenu" class="selected-menu-item">
						<div v-for="(list,index) in technology" :key="index" class="grid-items item1-hover">
							<span>
								<img :src="list.img" alt="">
							</span>
							<div :class="`item${navTitle.color}`">
								<label>{{list.title}}</label>
								<small><span v-if="list.sub">{{list.sub}}</span> {{list.text}}</small>
							</div>
						</div>
					</div>

					<div class="footer-mobile">
						<ul v-if="!selectedMenu">
							<li v-if="selectedNav != 'Technologies'" @click="toSelectNav('Technologies')">Technologies</li>
							<li v-if="selectedNav != 'Case Studies'" @click="toSelectNav('Case Studies')">Case Studies</li>
							<li v-if="selectedNav != 'Partners'" @click="toSelectNav('Partners')">Partners</li>
							<li v-if="selectedNav != 'Plans'" @click="toSelectNav('Plans')">Plans</li>
							<li v-if="selectedNav != 'Resources'" @click="toSelectNav('Resources')">Resources</li>
							<li v-if="selectedNav != 'Company'" @click="toSelectNav('Company')">Company</li>
						</ul>

						<div class="footer-button">
							<button>Contact Sales</button>
						</div>
					</div>
				</div>
			</transition>
    </header>
  </div>
</template>

<script>
export default {
	name: 'MegaMenu',
	data () {
		return {
			// technology: [],
			technology1: [
				{
					img: require('@/assets/img/mIDManagement.svg'),
					title: 'mIDManagement',
					sub: 'Next Gen',
					text: 'ID & Device Management'
				},
				{
					img: require('@/assets/img/mIDLogin.svg'),
					title: 'mIDLogin',
					sub: 'Next Gen',
					text: 'High Trust Login'
				},
				{
					img: require('@/assets/img/mIDFederation.svg'),
					title: 'mIDFederation',
					sub: 'Next Gen',
					text: 'Single Sign On'
				},
				{
					img: require('@/assets/img/mIDVerify.svg'),
					title: 'mIDVerify',
					sub: 'Next Gen',
					text: 'Multi-Factor Authentication'
				},
				{
					img: require('@/assets/img/mIDStart.svg'),
					title: 'mIDStart',
					sub: 'Next Gen',
					text: 'Digital Onboarding'
				},
				{
					img: require('@/assets/img/mIDRecovery.svg'),
					title: 'mIDRecovery',
					sub: 'Next Gen',
					text: 'Digital Access Recovery'
				},
			],
			technology2: [
				{
					img: require('@/assets/img/mChat.svg'),
					title: 'mChat',
					sub: 'Next Gen',
					text: 'Business Messaging'
				},
				{
					img: require('@/assets/img/mSign.svg'),
					title: 'mSign',
					sub: 'Next Gen',
					text: 'Digital Signature'
				},
				{
					img: require('@/assets/img/mPay.svg'),
					title: 'mPay',
					sub: 'Next Gen',
					text: 'Digital Payment'
				},
				{
					img: require('@/assets/img/mBusiness.svg'),
					title: 'mBusiness',
					sub: 'Next Gen',
					text: 'Business Process Automation'
				},
			],
			technology3: [
				{
					img: require('@/assets/img/signDot.svg'),
					title: 'signDot',
					sub: null,
					text: 'Tiny IoT of Trust'
				},
				{
					img: require('@/assets/img/signPod.svg'),
					title: 'signPod',
					sub: null,
					text: 'Next Gen IoT of Trust'
				},
				{
					img: require('@/assets/img/signPad.svg'),
					title: 'signPad',
					sub: null,
					text: 'Huge IoT of Trust'
				},
				{
					img: require('@/assets/img/signID.svg'),
					title: 'signID',
					sub: null,
					text: 'Secure IoT of Trust'
				},
			],
			technology4: [
				{
					img: require('@/assets/img/secOVID.svg'),
					title: 'secOVID',
					sub: null,
					text: 'OTP fit for the future'
				},
				{
					img: require('@/assets/img/secOPTIC.svg'),
					title: 'secOPTIC',
					sub: null,
					text: 'QR-Code Multi-Factor Authentication'
				},
			],
			navState: false,
			selectedNav: 'Technologies',
			selectedMenu: false,
			navTitle : {
				color: 0,
				title: ''
			},

		}
	}, methods : {
		toggleNav(type) {
			if(type == 'mobile') {
				this.selectedMenu = false;
			}
			this.navState = !this.navState;
		},
		toSelectNav(data) {
			this.selectedNav = data;
		},
		toSelectNavItem(color, title) {
			this.navTitle.color = color;
			this.navTitle.title = title;
			this.selectedMenu = !this.selectedMenu;
		},
	},
	computed: {
		technology : function () {
			if (this.navTitle.color == 1) {
				return this.technology1;
			}
			if (this.navTitle.color == 2) {
				return this.technology2;
			}
			if (this.navTitle.color == 3) {
				return this.technology3;
			}
			if (this.navTitle.color == 4) {
				return this.technology4;
			}
		}
	}

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@100;400;500;700&display=swap');


$color-default: #18182E;
$color-white: #fff;
$color-green-1: #15A2AB;
$color-green-2: #0DC5AB;

$color-blue: #489FFF;
$color-orange: #FD9D5D;
$color-gray: #9FA9BA;

$color-separator: #dfe5f291;

$bg-hover-green : #6ec5ca1a;
$bg-hover-blue : #489FFF1a;
$bg-hover-orange : #FD9D5D1a;
$bg-hover-gray : #9FA9BA1a;

body {
	background: linear-gradient(179.43deg, #F5F8FF 62.76%, #C0D7FF 168.3%);
	background-repeat: no-repeat;
	height: 100vh;
	color: $color-default;
}

// default transition
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}

// start of styles

.green-1 {
	color: $color-green-1;
}

.green-2 {
	color: $color-green-2;
}

.blue {
	color: $color-blue;
}

.orange {
	color: $color-orange;
}

.gray {
	color: $color-gray;
}

.mega-menu {
	
	position: relative;
	font-family: Barlow;
	max-width: 1440px;
	margin: 0 auto;
	padding-top: 48px;
	header {

		.hamburger {
			display: none;
		}
		
		nav {
			display:flex;
			justify-content: flex-end;
			margin-bottom: 20px;

			ul {
				display: flex;
				list-style-type: none;
				padding: 0;
			}

			li {
				font-family: Barlow;
				font-size: 15px;
				font-style: normal;
				font-weight: 400;
				line-height: 18px;
				letter-spacing: 0.5px;
				text-align: left;

				padding-left: 25px;
				cursor: default;
			}

			button {
				cursor: pointer;
				margin: 0 135px 0 142px;
				background: none;
				padding: 12px 40px;
				border: 1px solid $color-green-2;
				box-sizing: border-box;
				border-radius: 4px;
				
				color: $color-green-2;
				font-family: Barlow;
				font-size: 14px;
				font-style: normal;
				font-weight: 700;
				line-height: 17px;
				letter-spacing: 0.5px;
				text-align: center;

			}
		}

		.drop-down-container {
			:before {
				content: "\A";
				border-style: solid;
				border-width: 20px;
				border-color: transparent transparent $color-white transparent;
				position: absolute;
				top: -35px;
				left: 340px;
			}
			

			position: relative;
			
			max-width: 1170px;
			padding:30px 0;
			margin: 0 auto;
			background: $color-white;
			box-shadow: -10px 20px 60px rgba(110, 133, 168, 0.128141);
			border-radius: 12px;

			section {
				display: grid;
				grid-template-columns: 340px 295px 1fr 1fr;
				gap: 15px;
			}

			.menu-wrapper {
				display: grid;
				grid-template-columns: 340px 295px 1fr 1fr;
				gap: 15px;
			}
			.current-menu {
				display: none;
			}

			.header-mobile, .footer-mobile {
				display: none;
			}
			.grid-menu {
				font-family: Barlow;
				font-size: 16px;
				font-style: normal;
				font-weight: 500;
				line-height: 19px;
				letter-spacing: 1px;
				text-align: left;

				// padding-right: 25px;
				mix-blend-mode: normal;
				border-left: 1px solid $color-separator;
				padding: 0 10px 0 15px;

				.heading {
					font-family: Barlow;
					font-size: 18px;
					font-style: normal;
					font-weight: 600;
					line-height: 22px;
					letter-spacing: 0.5px;
					text-align: left;
					padding-bottom: 22.5px !important;

					.heading-wrap {
						display: flex;
					}
					.chevron-right {
						display: unset;
					}
					.chevron-right {
						display: none;
					}
				}

				.grid-items {
					display: flex;
					//transitions
					transition-property: all;
					transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
					transition-duration: 250ms;
					
					padding: 7.5px 20px;

					img, svg {
						padding-right: 10px;
					}

					small {
						font-size: 14px;
						font-weight: 400;
						span {
						font-weight: 600;
						}
					}
				}

				.item1, .item2, .item3, .item4{
					display: flex;
					flex-direction: column;
				}
				.item1 {
					span {
						color: $color-green-1;
					}
				}
				.item2 {
					span {
						color: $color-blue;
					}
				}
				.item3 {
					span {
						color: $color-orange;
					}
				}
				.item4 {
					span {
						color: $color-gray;
					}
				}

				.item1-hover:hover {
					background: $bg-hover-green;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.item2-hover:hover {
					background: $bg-hover-blue;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.item3-hover:hover {
					background: $bg-hover-orange;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.item4-hover:hover {
					background: $bg-hover-gray;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
			}

			.grid-menu:first-child {
				border-left: none;
			}

		}
	}
}

@media only screen and (max-width: 900px) {
	body {
		padding: 15px;
	}

	.flex-center {
		display: flex;
    align-items: center;
	}
	.mega-menu {
		header {

			.hamburger {
				display: block;
				text-align: right;
				padding: 0 15px;
			}

			nav {
				display: none;
			}

			.drop-down-container {
				:before {
					display: none;
				}

				position: absolute;
				display: grid;
				grid-template-columns: 1fr;
				width: 100%;
				top: 0;
				padding-top: 12px;

				section {
					display: block;
				}

				.current-menu {
					display: unset;
				}

				.menu-wrapper {
					position: absolute;
					grid-template-columns: 1fr;
				}

				.selected-menu-item {
					position: relative;
					background: $color-white;
					padding: 0 15px 0 10px;

					.grid-items {
						display: flex;
						//transitions
						transition-property: all;
						transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
						transition-duration: 250ms;
						
						padding: 15.5px 20px;

						img, svg {
							padding-right: 10px;
						}

						small {
							font-size: 14px;
							font-weight: 400;
							span {
							font-weight: 600;
							}
						}
					}

					.item1, .item2, .item3, .item4{
						display: flex;
						flex-direction: column;
					}
					.item1 {
						span {
							color: $color-green-1;
						}
					}
					.item2 {
						span {
							color: $color-blue;
						}
					}
					.item3 {
						span {
							color: $color-orange;
						}
					}
					.item4 {
						span {
							color: $color-gray;
						}
					}

					.item1-hover:hover {
						background: $bg-hover-green;
						mix-blend-mode: normal;
						border-radius: 10px;
						padding: 15.5px 20px;
					}
					.item2-hover:hover {
						background: $bg-hover-blue;
						mix-blend-mode: normal;
						border-radius: 10px;
						padding: 15.5px 20px;
					}
					.item3-hover:hover {
						background: $bg-hover-orange;
						mix-blend-mode: normal;
						border-radius: 10px;
						padding: 15.5px 20px;
					}
					.item4-hover:hover {
						background: $bg-hover-gray;
						mix-blend-mode: normal;
						border-radius: 10px;
						padding: 15.5px 20px;
					}
				}

				.grid-menu {
					.heading {
						justify-content: space-between;
						.heading-wrap {
							display: flex;
						}
						.chevron-right {
							display: unset;
						}
					}

					.menu-item {
						display: none;
					}
					
				}
				
				.header-mobile {
					display: flex;
					justify-content: space-between;
					align-items: center;
					padding-bottom: 36px;

					h2 {
						font-family: Barlow;
						font-size: 16px;
						font-style: normal;
						font-weight: 600;
						line-height: 20px;
						letter-spacing: 0px;
						text-align: left;

					}

					button {
						background: $color-green-2;
						padding: 12px 40px;
						color: $color-white;
						border-radius: 4px;
						border: none;
					}

					span {
						padding: 0 29px 0 26px;
					}
				}

				.current-menu {
					display: block;
					margin: 0 35px;
					color: #909DB2;
				}

				.footer-mobile {
					display: block;
					margin: 0 35px;
					padding-top: 35px;
					border-top: 1px solid #EDEDED;
					color: #173561;
					ul {
						display: grid;
						grid-template-columns: .5fr 1fr;
						gap: 24px;
						list-style-type: none;
						padding: 0;
					}

					li {
						font-family: Barlow;
						font-size: 16px;
						font-style: normal;
						font-weight: 400;
						line-height: 18px;
						letter-spacing: 0.5px;
						text-align: left;
						cursor: default;
					}
					
					button {
						display: none;
					}
				}
			}
		}
	}
}

@media only screen and (max-width: 640px) {
	body {
		padding: 15px;
	}
	.mega-menu {
		header {

			.hamburger {
				display: block;
				text-align: right;
				padding: 0 15px;
			}

			nav {
				display: none;
			}

			.drop-down-container {

				.header-mobile {
					button {
						display: none;
					}
				}

				.footer-mobile {

					button {
						display: unset;
						background: $color-green-2;
						padding: 11px 0;
						width: 100%;
						border-radius: 4px;
						border: none;
						color: $color-white;

						//font size
						font-family: Barlow;
						font-size: 14px;
						font-style: normal;
						font-weight: 700;
						line-height: 17px;
						letter-spacing: 0.5px;
						text-align: center;

					}
				}
			}
		}
	}
}




</style>
