import streamlit as st

# Page settings
st.set_page_config(page_title="ARC | DocChain", layout="centered", page_icon="📦")

# Background color (black) and text color (blue)
st.markdown("""
<style>
body {
background-color: black;
color: #00BFFF;
}
</style>
""", unsafe_allow_html=True)

st.title("ARC | DocChain Prototype")
st.subheader("Smart AI + Blockchain Export Document Manager")

# --- Company info form ---
st.header("Step 1: Company Information")
name = st.text_input("Company Name")
email = st.text_input("Email")
phone = st.text_input("Phone Number")
reg_no = st.text_input("Company Registration Number")

# --- Region selection ---
st.header("Step 2: Select Trade Region")
region = st.selectbox("Choose region", ["Select", "Asia", "Europe", "Middle East", "North America", "South America", "Africa"])

if region != "Select":
st.success(f"AI Recommendation: Documents needed for {region} exports include Invoices, Packing List, Bill of Lading, and Country-Specific Certificates.")

# --- Document upload ---
st.header("Step 3: Upload Trade Documents")
uploaded_files = st.file_uploader("Upload your trade documents (PDF, DOCX, etc.)", accept_multiple_files=True)

if uploaded_files:
for file in uploaded_files:
st.write(f"📄 {file.name} uploaded successfully.")

# --- AI Verification Simulation ---
st.header("Step 4: AI Verification")
if st.button("Run AI Verification"):
st.info("Analyzing documents for errors and inconsistencies...")
st.success("✅ All documents verified and blockchain-stamped for traceability!")

st.markdown("---")
st.caption("Powered by ARC | DocChain - Secure, Smart, Seamless Trade.")
