<html>
    <style>
        a {
            color:yellow;
        }
    </style>

    <script src="https://unimedrp--dev.sandbox.my.site.com/lightning/lightning.out.js"></script>
    </script>
    <div data-lightning-out="true"></div>

    <script>
        const appName = 'c:PartnerFormWrapper';
        const componentName = 'c:partnerForm';
        const lightningEndpoint = 'https://unimedrp--dev.sandbox.my.site.com/formularios/s/';
        const targetElement = document.querySelector("[data-lightning-out]");
        const componentAttributes = {

        };

        $Lightning.use(
            appName,
            function(){
                $Lightning.createComponent(
                    componentName,
                    componentAttributes,
                    targetElement,
                    function(cmp){
                        console.log('@cac funcionando');
                    }
                );
            },
            lightningEndpoint
        );
    </script>
</html>
