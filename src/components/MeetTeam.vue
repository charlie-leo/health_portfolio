<template>
  <section class="contact-section" id="contact">
    <h2>Contact & Resources</h2>
    <div class="contact-container">
      <div class="contact-column">
        <h3>University Services</h3>
        <ul>
          <li>
            <strong>University of Iowa UCS</strong><br>
            (319) 335‑7294 |
            <a href="https://counseling.uiowa.edu/additional-resources/resources-international-students" target="_blank">Website</a>
          </li>
          <li>
            <strong>University of Utah Counseling Center</strong><br>
            <a href="https://counselingcenter.utah.edu/resources/international-students.php" target="_blank">Website</a>
          </li>
          <li>
            <strong>CCA Global Crisis Hotline</strong><br>
            415‑551‑9344 |
            <a href="https://portal.cca.edu/thriving/caps/international-mental-health-support" target="_blank">Website</a>
          </li>
        </ul>
      </div>

      <div class="contact-column">
        <h3>Crisis Support</h3>
        <ul>
          <li><strong>Suicide & Crisis Lifeline (US & Canada)</strong><br> Dial 988</li>
          <li><strong>Crisis Text Line</strong><br>Text <b>HOME</b> to <b>741741</b></li>
        </ul>
      </div>

      <div class="contact-column">
        <h3>Online & Peer Support</h3>
        <ul>
          <li><strong>TalkCampus</strong> – <a href="https://www.talkcampus.com" target="_blank">Website</a></li>
          <li><strong>Active Minds</strong> – <a href="https://www.activeminds.org" target="_blank">Website</a></li>
          <li><strong>Westminster University Clinic</strong><br>📞 801‑832‑2910</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped>
.contact-section {
  background: #4e7575;
  color: #fff;
  padding: 2.5rem 1.5rem;
  border-radius: 0 0 12px 12px;
}

.contact-section h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
  text-align: center;
}

.contact-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 2rem;
}

.contact-column {
  flex: 1;
  min-width: 220px;
}

.contact-column h3 {
  font-size: 1.3rem;
  margin-bottom: 0.8rem;
  border-bottom: 1px solid #fff;
  padding-bottom: 0.4rem;
}

.contact-column ul {
  list-style: none;
  padding: 0;
}

.contact-column li {
  margin-bottom: 0.8rem;
  font-size: 0.95rem;
}

.contact-column a {
  color: #ffd700;
  text-decoration: none;
}

.contact-column a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .contact-container {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>
