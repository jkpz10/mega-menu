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

			<div class="drop-down-container">
				<div class="grid-menu">
					<div class="grid-items heading">
						mIDentity Line
					</div>
					<div class="grid-items item1">
						<label>mIDManagement</label>
						<small><span>Next Gen</span> ID & Device Management</small>
					</div>
					<div class="grid-items item1">
						<label>mIDLogin</label>
						<small><span>Next Gen</span> High Trust Login</small>
					</div>
					<div class="grid-items item1">
						<label>mIDManagement</label>
						<small><span>Next Gen</span> Single Sign On</small>
					</div>
					<div class="grid-items item1">
						<label>mIDManagement</label>
						<small><span>Next Gen</span> Multi-Factor Authentication</small>
					</div>
					<div class="grid-items item1">
						<label>mIDManagement</label>
						<small><span>Next Gen</span> Digital Onboarding</small>
					</div>
					<div class="grid-items item1">
						<label>mIDManagement</label>
						<small><span>Next Gen</span> Digital Access Recovery</small>
					</div>
				</div>
				<div class="grid-menu">
					<div class="grid-items heading">
						mPower Line
					</div>
					<div class="grid-items item2">
						<label>mChat</label>
						<small><span>Next Gen</span> Business Messaging</small>
					</div>
					<div class="grid-items item2">
						<label>mSign</label>
						<small><span>Next Gen</span> Digital Signature</small>
					</div>
					<div class="grid-items item2">
						<label>mPay</label>
						<small><span>Next Gen</span> Digital Payment</small>
					</div>
					<div class="grid-items item2">
						<label>mBusiness</label>
						<small><span>Next Gen</span> Business Process Automation</small>
					</div>
				</div>
				<div class="grid-menu">
					<div class="grid-items heading">
						Family
					</div>
					<div class="grid-items item3">
						<label>signDot</label>
						<small>Tiny IoT of Trust</small>
					</div>
					<div class="grid-items item3">
						<label>signPod</label>
						<small>Next Gen IoT of Trust</small>
					</div>
					<div class="grid-items item3">
						<label>signPad</label>
						<small><span>Next Gen</span> Single Sign On</small>
					</div>
					<div class="grid-items item3">
						<label>mIDManagement</label>
						<small>Huge IoT of Trust</small>
					</div>
					<div class="grid-items item3">
						<label>signID</label>
						<small>Secure IoT of Trust</small>
					</div>
				</div>
				<div class="grid-menu">
					<div class="grid-items heading">
						Technology
					</div>
					<div class="grid-items item4">
						<label>secOVID</label>
						<small>OTP fit for the future</small>
					</div>
					<div class="grid-items item4">
						<label>secOPTIC</label>
						<small>QR-Code Multi-Factor Authentication</small>
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

body {
	background: linear-gradient(179.43deg, #F5F8FF 62.76%, #C0D7FF 168.3%);
	background-repeat: no-repeat;
	height: 100vh;
}

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
			grid-template-columns: 29% 1fr 1fr 1fr;
			gap: 10px;

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
				padding: 0 15px;

				.heading {
					font-family: Barlow;
					font-size: 18px;
					font-style: normal;
					font-weight: 600;
					line-height: 22px;
					letter-spacing: 0.5px;
					text-align: left;
				}

				.item1:hover {
					background: $bg-hover-green;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.item2:hover {
					background: $bg-hover-blue;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.item3:hover {
					background: $bg-hover-orange;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.item4:hover {
					background: $bg-hover-gray;
					mix-blend-mode: normal;
					border-radius: 10px;
					padding: 7.5px 20px;
				}
				.grid-items {
					display: flex;
					flex-direction: column;

					//transitions
					transition-property: all;
					transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
					transition-duration: 250ms;

					padding: 7.5px 20px;

					small {
						font-size: 14px;
						font-weight: 400;
						span {
						font-weight: 600;
						}
					}
					
				}
			}

			.grid-menu:first-child {
				border-left: none;
			}
		}
	}
}


</style>
