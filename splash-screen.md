HTML CODE
<div class="splash">
  <div class="glow top"></div>
  <div class="glow bottom"></div>
  
  <div class="card">
    <div class="logo-icon">🧺</div>
    <h1 class="app-name">looma</h1>
    <p class="tagline">Made by hand. Sold with pride.</p>
  </div>

  <div class="actions">
    <button class="btn-main">Get Started</button>
    <p class="signin">Already have an account? <span>Sign in</span></p>
  </div>

  <p class="district">Nagaland · 17 Districts</p>
</div>

CSS CODE
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  min-height: 100vh;
  background: linear-gradient(160deg, #3B1408 0%, #8B3A2A 30%, #D4762A 65%, #E8A951 100%);
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  display: flex;
  align-items: center;
  justify-content: center;
}

.splash {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  width: 100%;
  position: relative;
  overflow: hidden;
}

.glow {
  position: absolute;
  border-radius: 50%;
  pointer-events: none;
}
.glow.top {
  width: 300px; height: 300px;
  top: -80px; right: -60px;
  background: radial-gradient(circle, rgba(240,192,96,0.25) 0%, transparent 70%);
}
.glow.bottom {
  width: 250px; height: 250px;
  bottom: 60px; left: -80px;
  background: radial-gradient(circle, rgba(139,58,42,0.4) 0%, transparent 70%);
}

.card {
  background: rgba(255,255,255,0.08);
  backdrop-filter: blur(24px);
  -webkit-backdrop-filter: blur(24px);
  border: 1px solid rgba(255,255,255,0.18);
  border-radius: 32px;
  padding: 56px 48px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 80%;
  max-width: 320px;
  box-shadow: 0 8px 48px rgba(0,0,0,0.3);
  animation: fadeUp 0.8s ease forwards;
}

.logo-icon {
  width: 72px; height: 72px;
  border-radius: 20px;
  background: linear-gradient(135deg, rgba(240,192,96,0.9), rgba(212,118,42,0.9));
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 34px;
  margin-bottom: 20px;
  box-shadow: 0 4px 20px rgba(240,192,96,0.4);
}

.app-name {
  color: #fff;
  font-size: 48px;
  font-weight: 700;
  letter-spacing: -1px;
  line-height: 1;
}

.tagline {
  color: rgba(255,255,255,0.65);
  font-size: 13px;
  margin-top: 10px;
  text-align: center;
  animation: fadeUp 0.8s ease 0.4s both;
}

.actions {
  margin-top: 40px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 12px;
  animation: fadeUp 0.8s ease 0.7s both;
}

.btn-main {
  background: linear-gradient(135deg, #F0C060, #D4762A);
  color: #3B1408;
  border: none;
  border-radius: 50px;
  padding: 16px 56px;
  font-size: 15px;
  font-weight: 700;
  cursor: pointer;
  box-shadow: 0 4px 24px rgba(240,192,96,0.45);
}

.signin {
  color: rgba(255,255,255,0.45);
  font-size: 12px;
}
.signin span {
  color: #F0C060;
  font-weight: 600;
  cursor: pointer;
}

.district {
  position: absolute;
  bottom: 28px;
  color: rgba(255,255,255,0.25);
  font-size: 11px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
}

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

JS CODE
// ready for next screen
