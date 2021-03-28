<script lang="ts">
    import firebase from "firebase/app";
    import "firebase/auth";
    import * as firebaseui from "firebaseui";

    const ui = new firebaseui.auth.AuthUI(firebase.auth());

    ui.start("#firebaseui-auth-container", {
        signInOptions: [
            {
                provider: firebase.auth.EmailAuthProvider.PROVIDER_ID,
                requireDisplayName: false
            }
        ]
    });

</script>
<div>
    <div id="firebaseui-auth-container"></div>
</div>
