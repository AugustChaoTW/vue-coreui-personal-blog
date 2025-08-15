<template>
  <div class="welcome">
    <ccontainer>
      <crow class="justify-content-center">
        <ccol md="8">
          <ccard class="shadow-sm">
            <ccardheader class="bg-primary text-white text-center">
              <h1 class="mb-0">
                <cicon class="me-2" icon="cilHome"></cicon>
                Welcome to Aug's Home
              </h1>
            </ccardheader>
            <ccardbody class="text-center p-5">
              <p class="lead mb-4">
                Welcome to Aug's Home
              </p>
            </ccardbody>
          </ccard>
        </ccol>
      </crow>
    </ccontainer>
  </div>
</template>

<script>
import {
  CContainer,
  CRow,
  CCol,
  CCard,
  CCardHeader,
  CCardBody,
  CIcon
} from '@coreui/vue'
import { cilHome } from '@coreui/icons'

export default {
  name: 'Welcome',
  components: {
    CContainer,
    CRow,
    CCol,
    CCard,
    CCardHeader,
    CCardBody,
    CIcon
  },
  setup() {
    return {
      cilHome
    }
  }
}
</script>

<style scoped>
.welcome {
  padding: 2rem 0;
  min-height: 100vh;
  background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
}

.card {
  border: none;
  border-radius: 15px;
  overflow: hidden;
}

.card-header {
  border-bottom: none;
  padding: 1.5rem;
}

.card-body {
  padding: 2rem;
}

h1 {
  font-weight: 600;
  font-size: 2rem;
}

.lead {
  font-size: 1.1rem;
  line-height: 1.6;
  color: #6c757d;
}
</style>
