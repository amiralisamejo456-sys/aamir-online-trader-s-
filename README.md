function sendToWhatsApp(e) {
    e.preventDefault();

    let name = document.getElementById("name").value;
    let product = document.getElementById("product").value;
    let details = document.getElementById("details").value;

    let message = `Name: ${name}%0AProduct: ${product}%0ADetails: ${details}`;

    let url = `https://wa.me/923342597609?text=${message}`;

    window.open(url, "_blank");
}
