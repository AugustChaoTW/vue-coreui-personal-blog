<template>
  <div class="home">
    <CContainer>
      <CRow class="justify-content-center">
        <CCol md="8">
          <CCard class="shadow-sm">
            <CCardHeader class="bg-primary text-white text-center">
              <h1 class="mb-0">
                <CIcon icon="cilHome" class="me-2" />
                Welcome to Aug's Home
              </h1>
            </CCardHeader>
            <CCardBody class="text-center p-5">
              <CAlert color="info" class="mb-4">
                <CIcon icon="cilInfo" class="me-2" />
                歡迎來到我的個人部落格！這里是使用 Vue.js 和 CoreUI 所建立的美麗網站。
              </CAlert>
              <p class="lead mb-4">
                這是一個使用了現代化技術所打造的個人網站，希望您在這里能多留連一會兒。
              </p>
              <div class="d-flex justify-content-center gap-3">
                <CButton color="primary" variant="outline">
                  <CIcon icon="cilUser" class="me-2" />
                  關於我
                </CButton>
                <CButton color="success" variant="outline">
                  <CIcon icon="cilEnvelopeClosed" class="me-2" />
                  聯繫我
                </CButton>
                <CButton color="info" variant="outline">
                  <CIcon icon="cilDescription" class="me-2" />
                  文章列表
                </CButton>
              </div>
            </CCardBody>
          </CCard>
        </CCol>
      </CRow>
    </CContainer>
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
  CAlert,
  CButton,
  CIcon
} from '@coreui/vue'
import { cilHome, cilInfo, cilUser, cilEnvelopeClosed, cilDescription } from '@coreui/icons'

export default {
  name: 'Home',
  components: {
    CContainer,
    CRow,
    CCol,
    CCard,
    CCardHeader,
    CCardBody,
    CAlert,
    CButton,
    CIcon
  },
  setup() {
    return {
      cilHome,
      cilInfo,
      cilUser,
      cilEnvelopeClosed,
      cilDescription
    }
  }
}
</script>

<style scoped>
.home {
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

.btn {
  border-radius: 25px;
  padding: 0.7rem 1.5rem;
  font-weight: 500;
  transition: all 0.3s ease;
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.alert {
  border: none;
  border-radius: 10px;
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
