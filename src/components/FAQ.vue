<template>
  <div class="page">
    <h1 style="margin-top: 120px; text-align: center;">FAQ</h1>

    <div class="faq">
      <div class="q" style="border-top: none;">
        <h5>Why is constructing an EV network important for rural areas?</h5>
        <p>
          Rural areas often lack access to reliable transportation. Establishing an EV network would improve transportation options, boost local economies, and improve environment sustainability.
        </p>
      </div>
      <div class="q">
        <h5>What initiatives are available to support Tribal Nations in developing renewable energy infrastructure for EV charging stations?</h5>
        <p style="padding-bottom: 0">
          Several organizations provide support:
        </p>
        <ul>
          <li>
            <strong>APPA</strong> collaborates with Tribal utilities to ensure access to affordable, reliable energy, aiding in the development of community-owned utilities that can establish EV charging infrastructure.
          </li>
          <li>
            <strong>NCAI</strong> promotes renewable energy integration and climate action initiatives tailored to Tribal communities.
          </li>
          <li>
            <strong>WAPA</strong> offers low-cost hydropower and grants for utility-scale projects, helping finance EV charging infrastructure.
          </li>
          <li>
            <strong>Tribal Solar Accelerator Fund</strong> provides grants specifically for Tribal solar energy projects, creating a sustainable power base for EV stations.
          </li>
          <li>
            <strong>Indian Energy</strong> works with Tribal Nations to develop solar, wind, and microgrid projects that can directly support EV infrastructure.
          </li>
        </ul>
      </div>
      <div class="q">
        <h5>Who can participate in the Initiative for Tribal Nations?</h5>
        <p>
          Federally recognized tribal nations and their governments are eligible to participate in the initiative. Partnerships with local organizations and agencies may also be facilitated to expand impact.
        </p>
      </div>
      <div class="q">
        <h5>How can tribal communities collaborate with local and national governments to implement EV infrastructure?</h5>
        <ul>
          <li>
            <strong>Engaging in discussions</strong> with local and state governments to advocate for supportive policies and funding for EV infrastructure projects.
          </li>
          <li>
            <strong>Applying for grants</strong> and incentives offered by federal and state agencies for EV adoption and infrastructure development.
          </li>
          <li>
            <strong>Working with transportation agencies</strong> to ensure that EV infrastructure is integrated into broader regional transportation planning and that the needs of tribal communities are represented.
          </li>
          <li>
            <strong>Creating cross-sector partnerships</strong> with other rural or indigenous communities to share resources, knowledge, and strategies for successful implementation.
          </li>
        </ul>
      </div>
      <div class="q">
        <h5>How are Native American tribes using renewable energy to promote energy sovereignty?</h5>
        <p>
          Native American tribes are actively pursuing energy sovereignty through renewable energy projects like solar and wind power. Initiatives by organizations such as Navajo Power and Solar Bear aim to combat energy poverty, create jobs, and reduce reliance on exploitative fossil fuel development. Federal legislation has provided funding to support these efforts and enable tribes to build sustainable, independent energy systems.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FAQ'
}
</script>

<style scoped>
.page {
  display: flex;
  flex-direction: column;
  color: white;
  width: 80%;
  margin: auto;
  font-size: 2vw;
  margin-bottom: 90px;
}

h5 {
  padding: 15px;
  font-size: 1.2vw;
  margin: 0;
}
p {
  padding: 15px;
  margin: 0;
  font-size: 20px;
  font-size: 1.3vw;
  color: rgba(255, 255, 255, 0.651);
}
li {
  color: rgba(255, 255, 255, 0.651);
  font-size: 20px;
  font-size: 1.3vw;
}

.faq {
  border: 1px solid rgba(255, 255, 255, 0.226);
}

.q {
  border-top: 1px solid rgba(255, 255, 255, 0.151);
}
</style>