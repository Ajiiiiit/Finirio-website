function calculateEMI() {
  const loan = document.getElementById("loan").value;
  const rate = document.getElementById("rate").value;
  const time = document.getElementById("time").value;
  const result = document.getElementById("emiResult");

  if (!loan || !rate || !time) {
    result.innerText = "Please fill all fields correctly!";
    return;
  }

  const P = loan;
  const R = rate / 12 / 100;
  const N = time * 12;

  const emi = (P * R * Math.pow(1 + R, N)) / (Math.pow(1 + R, N) - 1);
  result.innerText = "Monthly EMI: ₹" + emi.toFixed(2);
}
