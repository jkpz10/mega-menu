<template>
  <div class="mega-menu">
    <header>
      <nav>
        <ul>
          <li>Technologies</li>
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

			<div v-if="false" class="drop-down-container">
				<div class="grid-menu">
					<div class="grid-items heading green-1">
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
					<div class="grid-items item1-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#15A2AB"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M8.87662 14.1747C9.38649 12.8636 10.6489 12 12.0557 12V12C13.4624 12 14.7248 12.8636 15.2347 14.1747L15.5313 14.9372C15.543 14.9674 15.5207 15 15.4883 15H8.62301C8.59061 15 8.56833 14.9674 8.58007 14.9372L8.87662 14.1747Z" stroke="#15A2AB" stroke-width="1.5"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M12.0557 10C12.8841 10 13.5557 9.32843 13.5557 8.5C13.5557 7.67157 12.8841 7 12.0557 7C11.2272 7 10.5557 7.67157 10.5557 8.5C10.5557 9.32843 11.2272 10 12.0557 10Z" stroke="#15A2AB" stroke-width="1.5"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M5 6.76768C5 6.18543 5.39511 5.67743 5.95944 5.53411L11.3734 4.15913C11.7846 4.0547 12.2154 4.0547 12.6266 4.15913L18.0406 5.53411C18.6049 5.67743 19 6.18543 19 6.76768V11.7582C19 14.6333 17.3852 17.2647 14.8219 18.5667L12.9057 19.5399C12.3365 19.8291 11.6635 19.8291 11.0943 19.5399L9.17812 18.5667C6.61479 17.2647 5 14.6333 5 11.7582V6.76768Z" stroke="#15A2AB" stroke-width="1.5"/>
							</svg>
						</span>
						<div class="item1">
							<label>mIDManagement</label>
							<small><span>Next Gen</span> ID & Device Management</small>
						</div>
					</div>
					<div class="grid-items item1-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#15A2AB"/>
							<mask id="path-2-inside-1" fill="white">
							<rect x="5" y="5" width="14" height="6" rx="1"/>
							</mask>
							<rect x="5" y="5" width="14" height="6" rx="1" stroke="#15A2AB" stroke-width="3" mask="url(#path-2-inside-1)"/>
							<rect x="5" y="13" width="14" height="5" rx="1" fill="#15A2AB"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M9 9C9.55228 9 10 8.55228 10 8C10 7.44772 9.55228 7 9 7C8.44772 7 8 7.44772 8 8C8 8.55228 8.44772 9 9 9Z" fill="#15A2AB"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M12 9C12.5523 9 13 8.55228 13 8C13 7.44772 12.5523 7 12 7C11.4477 7 11 7.44772 11 8C11 8.55228 11.4477 9 12 9Z" fill="#15A2AB"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M15 9C15.5523 9 16 8.55228 16 8C16 7.44772 15.5523 7 15 7C14.4477 7 14 7.44772 14 8C14 8.55228 14.4477 9 15 9Z" fill="#15A2AB"/>
							</svg>
						</span>
						<div class="item1">
							<label>mIDLogin</label>
							<small><span>Next Gen</span> High Trust Login</small>
						</div>
					</div>
					<div class="grid-items item1-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#15A2AB"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M5 6.76768C5 6.18543 5.39511 5.67743 5.95944 5.53411L11.3734 4.15913C11.7846 4.0547 12.2154 4.0547 12.6266 4.15913L18.0406 5.53411C18.6049 5.67743 19 6.18543 19 6.76768V11.7582C19 14.6333 17.3852 17.2647 14.8219 18.5667L12.9057 19.5399C12.3365 19.8291 11.6635 19.8291 11.0943 19.5399L9.17812 18.5667C6.61479 17.2647 5 14.6333 5 11.7582V6.76768Z" stroke="#15A2AB" stroke-width="1.5"/>
							<rect x="9" y="11" width="6" height="4" rx="1" stroke="#15A2AB" stroke-width="1.5"/>
							<path d="M10.6665 11C10.6665 10.8702 10.6665 10.0597 10.6665 9.43403C10.6665 8.95135 10.8296 8.45927 11.2489 8.22011C11.4627 8.09811 11.7213 8 11.9998 8C12.2784 8 12.5369 8.09811 12.7508 8.22011C13.1701 8.45927 13.3332 8.95164 13.3332 9.43432V11" stroke="#15A2AB" stroke-width="1.5"/>
							</svg>
						</span>
						<div class="item1">
							<label>mIDManagement</label>
							<small><span>Next Gen</span> Single Sign On</small>
						</div>
					</div>
					<div class="grid-items item1-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#15A2AB"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M5 6.76768C5 6.18543 5.39511 5.67743 5.95944 5.53411L11.3734 4.15913C11.7846 4.0547 12.2154 4.0547 12.6266 4.15913L18.0406 5.53411C18.6049 5.67743 19 6.18543 19 6.76768V11.7582C19 14.6333 17.3852 17.2647 14.8219 18.5667L12.9057 19.5399C12.3365 19.8291 11.6635 19.8291 11.0943 19.5399L9.17812 18.5667C6.61479 17.2647 5 14.6333 5 11.7582V6.76768Z" stroke="#15A2AB" stroke-width="1.5"/>
							<path d="M9 12.1157L11.531 14.2519L16.1908 9" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							</svg>
						</span>
						<div class="item1">
							<label>mIDManagement</label>
							<small><span>Next Gen</span> Multi-Factor Authentication</small>
						</div>
					</div>
					<div class="grid-items item1-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#15A2AB"/>
							<rect x="5" y="5" width="14" height="13" rx="2" stroke="#15A2AB" stroke-width="1.5"/>
							<path d="M12 13.7331L13.4079 14.9214L16 12" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M8 11H11" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M8 8H14" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M8 14H9" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							</svg>
						</span>
						<div class="item1">
							<label>mIDManagement</label>
							<small><span>Next Gen</span> Digital Onboarding</small>
						</div>
					</div>
					<div class="grid-items item1-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#15A2AB"/>
							<path d="M10.6611 12.136L12.069 13.3243L14.6611 10.4028" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M6.81013 16.0159C9.13674 19.1034 13.5258 19.7202 16.6133 17.3936C19.7008 15.067 20.3176 10.678 17.991 7.59045C15.6644 4.50293 11.2754 3.88609 8.18787 6.21271" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M9.60001 15.6696L6.50922 15.6166L6.47708 18.8972" stroke="#15A2AB" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							</svg>
						</span>
						<div class="item1">
							<label>mIDManagement</label>
							<small><span>Next Gen</span> Digital Access Recovery</small>
						</div>
					</div>
				</div>
				<div class="grid-menu">
					<div class="grid-items heading blue">
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
					<div class="grid-items item2-hover">
						<span>
							<svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" x="0.5" width="24" height="24" rx="3" fill="#489FFF"/>
							<path fill-rule="evenodd" clip-rule="evenodd" d="M5.5 8C5.5 6.89543 6.39543 6 7.5 6H17.5C18.6046 6 19.5 6.89543 19.5 8V14.5C19.5 15.6046 18.6046 16.5 17.5 16.5H11.0684C10.6535 16.5 10.249 16.629 9.91069 16.8691L8.65767 17.7586C7.33335 18.6986 5.5 17.7517 5.5 16.1277V8Z" stroke="#489FFF" stroke-width="1.5"/>
							<path d="M9.58333 11.25H11.9167" stroke="#489FFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M14.8332 11.25H15.4165" stroke="#489FFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							</svg>
						</span>
						<div class="item2">
							<label>mChat</label>
							<small><span>Next Gen</span> Business Messaging</small>
						</div>
					</div>
					<div class="grid-items item2-hover">
						<span>
							<svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" x="0.5" width="24" height="24" rx="3" fill="#489FFF"/>
							<path d="M10.8182 7C7.88103 7 5.5 9.38103 5.5 12.3182C5.5 15.2553 7.88103 17.6364 10.8182 17.6364" stroke="#479EFE" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M10.818 12.3182H17.9089" stroke="#479EFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M15.545 9.95456L17.9086 12.3182" stroke="#479EFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							<path d="M15.545 14.6818L17.9086 12.3182" stroke="#479EFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
							</svg>
						</span>
						<div class="item2">
							<label>mSign</label>
							<small><span>Next Gen</span> Digital Signature</small>
						</div>
					</div>
					<div class="grid-items item2-hover">
						<span>
							<svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" x="0.5" width="24" height="24" rx="3" fill="#489FFF"/>
							<rect x="5.5" y="6" width="14" height="12" rx="2" stroke="#469DFF" stroke-width="1.5"/>
							<path d="M8.5 15H11.5" stroke="#469DFF" stroke-width="1.5" stroke-linecap="square"/>
							<path d="M5.5 10H18.5" stroke="#469DFF" stroke-width="1.5" stroke-linecap="square"/>
							</svg>
						</span>
						<div class="item2">
							<label>mPay</label>
							<small><span>Next Gen</span> Digital Payment</small>
						</div>
					</div>
					<div class="grid-items item2-hover">
						<span>
							<svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" x="0.5" width="24" height="24" rx="3" fill="#489FFF"/>
							<rect x="5.5" y="9" width="14" height="9" rx="2" stroke="#469DFF" stroke-width="1.5"/>
							<path d="M9 12.5H16" stroke="#469DFF" stroke-width="1.5" stroke-linecap="square"/>
							<path d="M8.5 8V8C8.5 6.89543 9.39543 6 10.5 6H14.5C15.6046 6 16.5 6.89543 16.5 8V8" stroke="#469DFF" stroke-width="1.5" stroke-linecap="square"/>
							</svg>
						</span>
						<div class="item2">
							<label>mBusiness</label>
							<small><span>Next Gen</span> Business Process Automation</small>
						</div>
					</div>
				</div>
				<div class="grid-menu">
					<div class="grid-items heading orange">
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
					<div class="grid-items item3-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#FD9D5D"/>
							<rect x="5" y="6" width="14" height="12" rx="2" stroke="#FD9D5D" stroke-width="1.5"/>
							<path d="M5 8C5 6.89543 5.89543 6 7 6H17C18.1046 6 19 6.89543 19 8V14H5V8Z" stroke="#FD9D5D" stroke-width="1.5"/>
							</svg>
						</span>
						<div class="item3">
							<label>signDot</label>
							<small>Tiny IoT of Trust</small>
						</div>
					</div>
					<div class="grid-items item3-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#FD9D5D"/>
							<rect x="7" y="5" width="10" height="15" rx="2" stroke="#FD9D5D" stroke-width="1.5"/>
							<path d="M7 7C7 5.89543 7.89543 5 9 5H15C16.1046 5 17 5.89543 17 7V17H7V7Z" stroke="#FD9D5D" stroke-width="1.5"/>
							<rect x="11" y="17" width="2" height="3" fill="#FD9D5D"/>
							</svg>
						</span>
						<div class="item3">
							<label>signPod</label>
							<small><span>Next Gen</span> IoT of Trust</small>
						</div>
					</div>
					<div class="grid-items item3-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#FD9D5D"/>
							<rect x="5" y="5" width="14" height="14" rx="2" stroke="#FD9D5D" stroke-width="1.5"/>
							<path d="M5 7C5 5.89543 5.89543 5 7 5H16V19H7C5.89543 19 5 18.1046 5 17V7Z" stroke="#FD9D5D" stroke-width="1.5"/>
							</svg>
						</span>
						<div class="item3">
							<label>signPad</label>
							<small>Huge IoT of Trust</small>
						</div>
					</div>
					<div class="grid-items item3-hover">
						<span>
							<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect opacity="0.1" width="24" height="24" rx="3" fill="#FD9D5D"/>
							<rect x="8" y="3" width="8" height="18" rx="2" stroke="#FD9D5D" stroke-width="1.5"/>
							<path d="M8 5C8 3.89543 8.89543 3 10 3H14C15.1046 3 16 3.89543 16 5V16H8V5Z" stroke="#FD9D5D" stroke-width="1.5"/>
							<rect x="11" y="19" width="2" height="2" fill="#FD9D5D"/>
							</svg>
						</span>
						<div class="item3">
							<label>signID</label>
							<small>Secure IoT of Trust</small>
						</div>
					</div>
				</div>
				<div class="grid-menu">
					<div class="grid-items heading gray">
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
					<div class="grid-items item4-hover">
						<span>
							<svg width="18" height="10" viewBox="0 0 18 10" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect x="17" y="1" width="8" height="16" rx="2" transform="rotate(90 17 1)" stroke="#9FA9BB" stroke-width="1.5"/>
							<path d="M15 1C16.1046 1 17 1.89543 17 3V7C17 8.10457 16.1046 9 15 9L6 9L6 1L15 1Z" stroke="#9FA9BB" stroke-width="1.5"/>
							<path d="M3.50439 6V4" stroke="#9FA9BB" stroke-width="1.5"/>
							</svg>
						</span>
						<div class="item4">
							<label>secOVID</label>
							<small>OTP fit for the future</small>
						</div>
					</div>
					<div class="grid-items item4-hover">
						<span>
							<svg width="10" height="17" viewBox="0 0 10 17" fill="none" xmlns="http://www.w3.org/2000/svg">
							<rect x="1" y="1" width="8" height="15" rx="2" stroke="#9FA9BB" stroke-width="1.5"/>
							<path d="M1 3C1 1.89543 1.89543 1 3 1H7C8.10457 1 9 1.89543 9 3V13H1V3Z" stroke="#9FA9BB" stroke-width="1.5"/>
							</svg>
						</span>
						<div class="item4">
							<label>secOPTIC</label>
							<small>QR-Code Multi-Factor Authentication</small>
						</div>
					</div>
				</div>
			</div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'MegaMenu',
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
	
	font-family: Barlow;
	max-width: 1440px;
	margin: 0 auto;
	padding-top: 48px;
	header {
		
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
			display: grid;
			grid-template-columns: 340px 295px 1fr 1fr;
			gap: 15px;

			max-width: 1170px;
			padding:30px 0;
			margin: 0 auto;
			background: $color-white;
			box-shadow: -10px 20px 60px rgba(110, 133, 168, 0.128141);
			border-radius: 12px;


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
				}

				.grid-items {
					display: flex;
					//transitions
					transition-property: all;
					transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
					transition-duration: 250ms;
					
					padding: 7.5px 20px;

					svg {
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


</style>
