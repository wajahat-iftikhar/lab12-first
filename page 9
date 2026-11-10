
const form = document.querySelector("#orderForm");

if (form) {

    form.addEventListener("submit", function(event) {

        event.preventDefault();

        if (!form.reportValidity()) {
            return;
        }

        const name = document.querySelector("#customer").value.trim();

        const quantity = Number(
            document.querySelector("#quantity").value
        );

        const price = 10000;

        const total = quantity * price;

        const notice = document.querySelector("#confirmation");

        notice.textContent =
            "Thank you, " + name +
            "! Your order request for " +
            quantity + " watch(es) has been prepared. " +
            "Total Price: PKR " +
            total.toLocaleString("en-PK") +
            ". No order was actually sent.";

        notice.style.display = "block";

    });

}
