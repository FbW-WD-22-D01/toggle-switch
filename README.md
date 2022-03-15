# Ein einfacher toggle switch

Im Code findet ihr noch Kommentierungen. Der toggle switch ist ganz simpel ohne Animationen. Online findet ihr zig verschiedene Varianten.

*html:*

    <div>
        <input type="checkbox" id="toggle" name="checkbox-toggle">
        <label for="toggle"></label>
    </div>

*css:*

    label {
        position: relative;
        display: inline-block;
        width: 40px;
        height: 20px;
        background-color: gray;
        border-radius: 20px;
    }



    label::before {
        content: "";
        position: absolute;
        width: 18px;
        height: 18px;
        border-radius: 50%;
        background-color: white;
        top: 1px;
        left: 1px;
    }

    input:checked + label::before {
        left: 20px;
    }

    input {
        display: none;
    }