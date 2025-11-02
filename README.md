/* Variables */
:raíz {
    --primario-r: 0;
    --primary-g: 164;
    --primario-b: 220;
    --color-acento-primario: rgba(var(--primario-r), var(--primario-g), var(--primario-b), 1.0);
    --color-de-acento-secundario: #00a4dc20;
    --color-de-fondo-primario: transparent;
    --color-de-fondo-secundario: #181818;
    --fondo-primario-transparente: rgba(35,35,35,0.5);
    --secondary-background-transparent: rgba(0,0,0,0.6);
    --tarjetas-redondeadas: 15px;
    --blur: 10px;

    /* Acentos alternativos */
    --primary-alt1: rgb(calc(var(--primary-r) - 30), calc(var(--primary-g) - 30), calc(var(--primary-b) - 30), 1);
    --primary-alt2: rgb(calc(var(--primary-r) - 30), calc(var(--primary-g) - 30), calc(var(--primary-b) - 30), 0,85);
    --primary-alt3: rgb(calc(var(--primary-r) - 30), calc(var(--primary-g) - 30), calc(var(--primary-b) - 30), 0.7);
    --primary-alt4: rgb(calc(var(--primary-r) - 30), calc(var(--primary-g) - 30), calc(var(--primary-b) - 30), 0,55);
    --primary-alt5: rgb(calc(var(--primary-r) - 30), calc(var(--primary-g) - 30), calc(var(--primary-b) - 30), 0.4);
}

/* Configurando la variable de color de acento */
.emby-checkbox:checked + span + .checkboxOutline,
.panelComandosDeSelección,
.indicador de conteo,
.MuiButton-root.MuiButton-containedSizeMedium,
.MuiChip-root.MuiChip-colorInfo:not(.MuiChip-colorError),
progreso[aria-valuenow]:antes {
    fondo: var(--color-de-acento-primario) !importante;
}
progreso::-moz-barra-de-progreso {
    fondo: var(--color-de-acento-primario) !importante;
}
progreso::-webkit-progreso-valor {
    fondo: var(--color-de-acento-primario) !importante;
}
.MuiAlert-root.MuiAlert-standardInfo {
    fondo: var(--color-de-acento-secundario) !importante;
}
.emby-checkbox:checked + span + .checkboxOutline,
.emby-checkbox:focus:not(:checked) + span + .checkboxOutline,
.emby-input:focus,
.emby-textarea:focus,
.emby-select-withcolor:focus,
.mdl-spinner__capa-1,
.mdl-spinner__capa-2,
.mdl-spinner__capa-3,
.mdl-spinner__capa-4,
.anillo-de-progreso {
    color-border: var(--color-acento-primario) !important;
}
.page:not(.itemDetailPage) .button-link,
.selectLabelFocused,
.textareaLabelFocused,
.inputLabelFocused,
.emby-tab-button:hover,
.metadataSidebarIcon,
.upNextDialog-countdownText,
.MuiSvgIcon-root.MuiSvgIcon-fontSizeInherit,
.listItemImageButton:hover,
.button-flat:hover,
#divRunningTasks span {
    color: var(--color-de-acento-primario) !importante;
}
@media (hover: hover) and (pointer: fine) {
    .paper-icon-button-light:hover:not(:disabled) {
        color: var(--color-de-acento-primario) !importante;
        background-color: var(--secondary-accent-color) !important;
    }
}

/* Aumentar el tamaño del logotipo de Jellyfin */
.layout-desktop .pageTitleWithLogo {
    margen izquierdo: 25px !importante;
    altura: 40px !importante;
}

/* Corrección para encabezado vacío con relleno */
[dir="ltr"] .pageTitle:not(.pageTitleWithLogo):empty {
    margen: 0 !importante;
}

/* Cajón izquierdo estático */
.layout-desktop .mainDrawer {
    izquierda: 0 !importante;
    superior: 0 !importante;
    ancho: 250px !importante;
    /* Color de fondo modificado */
    fondo: var(--color-de-fondo-secundario) !importante;
    /* Mover el cajón detrás del encabezado */
    índice z: 998 !importante;
}
/* Botones del cajón inferior */
.layout-desktop .mainDrawer-scrollContainer {
    margen superior: 95px !importante;
    margen izquierdo: 10px !importante;
}
.layout-mobile .mainDrawer-scrollContainer {
    margen superior: 15px !importante;
}
/* Desplazar el contenido a la derecha */
.layout-desktop .libraryPage:not(#editItemMetadataPage) {
    margen izquierdo: 250px !importante;
}
/* Corrección para Jellyfin Media Player */
.quickConnectSettingsContainer {
    margen izquierdo: 250px !importante;
}
/* Ocultar la transición al cargar la página */
.layout-desktop .touch-menu-la.transition {
    transición: ninguna !importante;
}
/* Ocultar botón de hamburguesa */
.layout-desktop .mainDrawerButton {
    mostrar: ninguno !importante;
}
/* Corrección para el problema de la fuga de información del panel de control fuera de las secciones */
.columnaDelTablero {
    flex-shrink: heredar;
}
/* Corrección para la altura del botón del cajón del panel de control */
.layout-desktop .dashboardDocument .mainDrawer-scrollContainer {
    relleno-superior: 0 !importante;
}
/* Ocultar botón de inicio */
.layout-desktop .headerHomeButton {
    mostrar: ninguno !importante;
}
.layout-desktop .dashboardDocument .headerHomeButton {
    mostrar: bloque !importante;
}
/* Corrección para el reproductor de vídeo y la página de inicio de sesión */
.diseño-escritorio .ocultar-desplazamiento .cajón-principal,
.layout-desktop .hideMainDrawer .mainDrawer {
    izquierda: -320px !importante;
}
/* Corrección para la desalineación de los elementos de la colección */
.layout-desktop .collectionItems .collectionItemsContainer {
    relleno-izquierda: 0% !importante;
}
.layout-desktop .collectionItems .sectionTitleContainer {
    relleno-izquierda: 0% !importante;
}
/* Botones dinámicos */
.layout-desktop .navMenuOption:hover:not(.navMenuOption-selected) {
    transformar: escala(1.05) !importante;
}
.layout-desktop .listItem {
    transición: .2s !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
.layout-desktop #myPreferencesMenuPage .listItem:hover {
    transformación: escala(1.015);
}



/* Tarjetas redondeadas */
.cardContent,
.cardPadder,
.cardOverlayContainer,
.blurhash-canvas,
.diálogo,
.itemSelectionPanel,
.nowPlayingPageImage {
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
/* Menú de selección redondeado */
.itemSelectionPanel {
    borde: 2px sólido var(--color-de-acento-primario) !importante;
}
.itemSelectionPanel .checkboxOutline {
    margen: 7px !importante;
}



/* Barra de progreso flotante */
.innerCardFooter {
    borde-radio: var(--tarjetas-redondeadas) !importante;
    margen izquierdo: 5px !importante;
    margen inferior: 5px !importante;
    relleno: 5px 15px 5px 5px !importante;
    abajo: 0% !importante;
    fondo: rgba(0,0,0,0.5) !importante;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.fullInnerCardFooter {
    abajo: 5% !importante;
    ancho: 90% !importante;
    margen: auto !importante;
    borde-radio: 100px !importante;
    relleno: 0px !importante;
    filtro de fondo: ninguno !importante;
}
.itemProgressBar:not(.playbackProgress):not(.transcodingProgress):not(.backgroundProgress) {
    altura: 10px !importante;
    fondo: var(--primary-background-transparent) !important;
    filtro de fondo: desenfoque(2px) !importante;
    borde-radio: 100px !importante;
}
.innerCardFooterClear {
    background-color: none !important;
}
.innerCardFooter .cardText {
    relleno: 0 0 0 10px !importante
}
.cardImageContainer .innerCardFooter .itemProgressBar .itemProgressBarForeground {
    fondo: var(--color-de-acento-primario) !importante;
}
.itemProgressBarForeground {
    borde-radio: 100px !importante;
}
.transcodingProgress > div {
    background-color: hsla(0,0%,100%,.2) !important;
}
.activeSession .backgroundProgress,
.activeSession .playbackProgress,
.activeSession .transcodingProgress {
    abajo: 10px !importante;
    borde-radio: 100px !importante;
    ancho: 90% !importante;
    izquierda: 5% !importante;
}
.sessionNowPlayingInnerContent {
    relleno inferior: 12px !importante;
    relleno en línea: 17px !important;
}
.sessionAppInfo {
    relleno: .5em 0em !importante;
}
.sessionNowPlayingInfo {
    relleno: .8em 0em !importante;
}



/* Indicador verde vigilado */
.indicadorreproducido {
    fondo: #409843 !importante;
}



/* Botones redondeados del cajón izquierdo */
.navMenuOption,
.navMenuOption:hover,
.navMenuOption-selected {
    borde-radio: 100px !importante;
    ancho: 85% !importante;
    margen: auto !importante;
    alineación del texto: centro !importante;
    altura: 45px !importante;
    margen superior: 3px !importante;
    margen inferior: 3px !importante;
}
.navMenuOption:hover:not(.navMenuOption-selected) {
    color de fondo: rgba(44, 44, 44, 0.7);
}
/* Centrar iconos y texto y desplazar a la izquierda */
.navMenuOptionIcon,
.navMenuOptionText {
    posición: heredar !importante;
    izquierda: -10% !importante;
    margen superior: 0 !importante;
}
/* Corrección para los botones del encabezado */
.layout-desktop .emby-button-foreground {
    arriba: -9px !importante;
}
.layout-tv .emby-button-foreground {
    arriba: -14px !importante;
}



/* Color de botón personalizado */
.navMenuOption-selected {
    fondo: var(--color-de-acento-secundario) !importante;
    color: var(--color-de-acento-primario) !importante;
}

/* Color de fondo modificado */
html,
.contenedordefondo:no(.confondo):no(.contenedordefondo-transparente),
.noBackdropTransparency .detailPageSecondaryContainer {
    color de fondo: var(--color-de-fondo-primario) !importante;
}


/* Barra de encabezado transparente */
.skinHeader {
    color de fondo: transparente !importante;
}
.layout-desktop .skinHeader,
.layout-tv .skinHeader {
    relleno superior: 1,5em !importante;
}
.layout-tv .skinHeader {
    relleno inferior: 10px !importante;
}
/* Botones de encabezado redondeados */
.headerTabs,
.headerRight {
    background-color: var(--primary-background-transparent) !important;
    borde-radio: 50px !importante;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.layout-desktop .headerTabs,
.layout-tv .headerTabs {
    margen inferior: 10px !importante;
}
.layout-desktop .headerTabs {
    margen izquierdo: 160px !importante;
    margen superior: -58px !importante;
}
/* Altura del botón */
.headerRight,
.emby-tab-button {
    altura: 45px !importante;
}
/* Bajar el encabezado y añadir relleno a los botones de la derecha */
.layout-desktop .headerRight {
    relleno: 0px 5px !importante;
}
.layout-tv .headerRight {
    relleno: 20px 10px !importante;
}
/* Volver a subir el encabezado izquierdo */
.layout-desktop .headerLeft
.layout-tv .headerLeft {
    posición: relativa !importante;
    arriba: -17px !importante;
}
/* Correcciones para móviles */
.layout-mobile .headroom--unpinned {
    transformar: traslaciónY(-50%);
}
.layout-mobile .sectionTabs {
    margen-izquierda: auto !importante;
    margen-derecha: auto !importante;
    ancho: auto !importante;
    ancho-máximo: 100% !importante;
}
.layout-mobile .emby-button-foreground {
    arriba: -2px !importante;
}
.layout-mobile .skinHeader {
    transición: .1s !importante;
}
.layout-mobile .mainDrawer {
    fondo: var(--color-de-fondo-secundario) !importante;
}
.layout-mobile .headroom--unpinned {
    transformación: ninguna;
}
.layout-mobile .headroom--unpinned:has(.headerTabs.sectionTabs:not(.hide)) {
    transformar: traslaciónY(-50%);
}
.layout-mobile .headroom--not-top {
    fondo: var(--primary-background-transparent) !important;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.layout-mobile .headroom--not-top .headerRight {
    Antecedentes: ninguno !importante;
}
.layout-mobile .headroom--superior,
.layout-mobile .headroom--not-top:has(.headerTabs.sectionTabs:not(.hide)) {
    fondo: transparente !importante;
    filtro de fondo: ninguno !importante;
}
.layout-mobile .headroom--top .headerRight ,
.layout-mobile .headroom--not-top:has(.headerTabs.sectionTabs:not(.hide)) .headerRight {
    fondo: var(--primary-background-transparent) !important;
}
@media (max-width: 380px) {
    .layout-mobile .pageTitle:not(.pageTitleWithLogo):not(:empty) {
        posición: ¡absoluta!importante;
        margen-izquierda: 50% !importante;
        transformar: traducir(-50%, 0) !importante;
        arriba: 60px !importante;
    }
    .layout-mobile .headerTop:has(.pageTitle:not(.pageTitleWithLogo):not(:empty)) {
        -webkit-align-items: inicio !important;
        alinear-elementos: empezar !importante;
    }
    .layout-mobile .skinHeader:has(.pageTitle:not(.pageTitleWithLogo):not(:empty)) {
        altura: 110px !importante;
    }
    .layout-mobile .skinHeader:has(.pageTitle:not(.pageTitleWithLogo):not(:empty)):has(.sectionTabs:not(.hide)) {
        altura: 140px !importante;
    }
    .layout-mobile .libraryPage:not(.noSecondaryNavPage) {
        relleno superior: 9,5em !importante;
    }
    .layout-mobile .headroom--unpinned:has(.headerTabs.sectionTabs:not(.hide)):has(.pageTitle:not(.pageTitleWithLogo):not(:empty)) {
        transformar: traslaciónY(-60%);
    }
}



/* Modificaciones del jugador */
.upNextContainer:not(#skipIntro), .toastVisible {
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.upNextContainer:no(#skipIntro) {
    borde-radio: var(--tarjetas-redondeadas) !importante;
    background-color: rgba(0, 0, 0, 0.6) !important;
}
.upNextContainer {
    margen: 4% !importante;
}
.toastVisible {
    borde-radio: 30px !importante;
    background-color: var(--primary-background-transparent) !important;
}
.sliderBubble {
    borde-radio: var(--tarjetas-redondeadas) !importante;
    background-color: var(--secondary-background-transparent) !important;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.sliderBubble:not(.osdVolumeSliderContainer .sliderBubble):has(.chapterThumbContainer) {
    background-color: #ffffff00 !important;
    arriba: 25px !importante;
    filtro de fondo: ¡desactivado!importante;
}
@supports selector(div:not(.parent .child)) {
    .mdl-slider-background-flex:not(.layout-mobile .nowPlayingBar .mdl-slider-background-flex) {
        altura: 10px !importante;
        margen superior: -5px !importante;
        borde-radio: 100px !importante;
        fondo: hsla(0,0%,100%,.2) !importante;
    }
}
@supports no selector(div:not(.parent .child)) {
    .mdl-slider-background-flex {
        altura: 10px !importante;
        margen superior: -5px !importante;
        borde-radio: 100px !importante;
        fondo: hsla(0,0%,100%,.2) !importante;
    }
}
.mdl-slider-background-lower {
    borde-radio: 100px !importante;
    color de fondo: var(--color-de-acento-primario) !importante;
}
/* Moz */
.mdl-slider::-moz-range-thumb {
    fondo: #ffffff00 !importante;
    altura: 10px !importante;
    ancho: 8px !importante;
    borde-radio: 2px !importante;
}
.mdl-slider-hoverthumb:hover::-moz-range-thumb {
    transformación: escalaY(2);
    fondo: #fff !importante;
}
/* Webkit */
.mdl-slider::-webkit-slider-thumb {
    fondo: #ffffff00 !importante;
    altura: 10px !importante;
    ancho: 8px !importante;
    borde-radio: 2px !importante;
}
.mdl-slider-hoverthumb:hover::-webkit-slider-thumb {
    transformación: escalaY(2);
    fondo: #fff !importante;
}

.mdl-slider-background-upper {
    borde-superior-derecho-radio: 100px !importante;
    borde-inferior-derecho-radio: 100px !importante;
    fondo: hsla(0,0%,100%,.2) !importante;
    transformar: translateX(-3px) !important;
}
.iconOsdProgressInner {
    fondo: var(--color-de-acento-primario) !importante;
}

/* Siguiente carta */
.botones-siguiente-diálogo .botón-siguiente-diálogo {
    transición: .2s !importante;
}
.upNextDialog-buttons .upNextDialog-button:hover {
    transformación: escala(1.1);
}

/* Compatibilidad con el plugin Jellyscrub */
.chapterThumbContainer {
    Antecedentes: ninguno !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
    box-shadow: unset !important;
}
.capítuloMiniatura {
    borde-radio: var(--tarjetas-redondeadas) !importante;
    margen inferior: 47px !importante;
    box-shadow: 0 0 1.9vh #000 !important;
}
.chapterThumbTextContainer {
    Antecedentes: ninguno !importante;
}
.chapterThumbText {
    alineación del texto: centro !importante;
}
.chapterThumbText-dim {
    mostrar: ninguno !importante;
}

/* Compatibilidad con el plugin IntroSkipper */
#omitirIntroducción .btnOmitirIntroducción {
    transición: 0,2 s;
    borde-radio: 100px !importante;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
#skipIntro .btnSkipIntro:hover {
    transición: .2s;
    transformación: escala(1.05);
    fondo: var(--color-de-acento-primario) !importante;
}
#skipIntro .paper-icon-button-light:hover:not(:disabled) {
    color: #FFF !importante;
}
.sliderContainer:has(.mdl-slider-hoverthumb:not(:hover)) .sliderMarker {
    opacidad: 0 !importante;
    transición: 0.2s !importante;
}
.sliderContainer:has(.mdl-slider-hoverthumb:hover) .sliderMarker {
    opacidad: 1 !importante;
    transición: 0.2s !importante;
    altura: 10px !importante;
    transformar: translate3d(0,40%,0) !importante;
    -webkit-transform: translate3d(0,40%,0) !important;
}
.sliderMarker.watched {
    background-color: #FFFFFF90 !important;
    índice z: 10 !importante;
}
#omitirIntroducción .upNextContainer {
    relleno: 0px !importante;
}
#omitirIntroducción .emby-button {
    fondo: rgba(30, 30, 30, 0.7) !importante;
}
#skipIntro .emby-button:hover {
    box-shadow: 0 0 8px rgba(var(--primary-accent-color), 0.6) !important;
}
#skipIntro .emby-button:focus {
    fondo: rgba(30, 30, 30, 0.7) !importante;
    box-shadow: unset !important;
}
/* Compatibilidad con el plugin InPlayerEpisodePreview */
.layout-desktop #popupFocusContainer {
    relleno: 10px !importante;
}
.layout-desktop #popupTitleContainer {
    margen: 0px !importante;
    relleno: 10px 0px 10px 0px !importante;
}
.layout-desktop #popupContentContainer .previewEpisodeDetails {
    posición: sin definir !importante;
    margen: 0px 0px 6px 10px !importante;
    tamaño de fuente: 13,5px !importante;
}
.layout-desktop #popupContentContainer .previewEpisodeTitle {
    tamaño de fuente: 16,5px !importante;
}
.layout-desktop #popupContentContainer .listItem {
    relleno: .25em .25em .25em .5em !importante;
}

/* Modificar botones del reproductor */
.material-icons.fast_rewind::before {
    contenido: "\e059";
}
.material-icons.fast_forward::before {
    contenido: "\e057";
}
.material-icons.audiotrack::before {
    contenido: "\e91f";
}



/* Modificaciones de configuración y panel de control */
.emby-input,
.emby-textarea,
.paperList,
.listItem:hover,
.subtitleappearance-preview {
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
.botón-enviar,
.emby-select,
.checkboxOutline,
.btnActualizar,
#btnCierre
.aumentó {
    borde-radio: 100px !importante;
}
.botón-enviar {
    fondo: var(--color-de-acento-primario) !importante;
}
/* Modificar la ubicación del nombre de usuario en la página de perfil */
.layout-desktop #userProfilePage .readOnlyContent div:not([class]), div[class=""]{
    alinear elementos: inicial !importante;
}
.layout-desktop .username {
    margen: 0px 0px 10px 10px !importante;
}
/* Botón rojo de apagado */
#btnShutdown {
    fondo: #AE3739 !importante;
}
/* Eliminar el borde debajo de ciertos elementos del panel de control */
.listItem-border {
    borde: 0 !importante;
}
/* Agregar relleno a los elementos de la lista */
.layout-desktop .listItem,
.layout-tv .listItem {
    relleno en línea: 15px !important;
}
/* Tarjetas de panel redondeadas */
.cardBox {
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
/* Se eliminó la fealdad del estilo de la tarjeta de borde */
.layout-desktop fieldset.verticalSection-extrabottompadding,
.layout-tv fieldset.verticalSection-extrabottompadding {
    borde-radio: var(--tarjetas-redondeadas) !importante;
    color de borde: #3B3B3B !importante;
    relleno: 10px 35px !importante;
}
/* Selección de pestañas redondeadas en el panel de control */
.layout-desktop .localnav {
    borde-radio: 100px !importante;
    Antecedentes: #202020 !importante;
    ancho: ajustar-contenido !importante;
}
.layout-desktop a[data-role="button"] {
    Antecedentes: ninguno !importante;
}
.layout-desktop div[data-role="controlgroup"] a.ui-btn-active {
    fondo: var(--color-de-acento-primario) !importante;
    borde-radio: 100px !importante;
}
.layout-desktop .dashboardDocument .mainAnimatedPage {
    izquierda: 260px !importante;
}
#página de visualización de la biblioteca,
#metadataImagesConfigurationPage,
#metadataNfoPage {
    margen superior: 40px !importante;
}
#mediaLibraryPage {
    margen superior: 10px !importante;
}
/* Realinear dispositivos activos en el panel de control */
.activeDevices.itemsContainer {
    margen: 0px !importante;
}
.playbackProgress > div {
    fondo: var(--color-de-acento-primario) !importante;
}
/* Configuración de IntroSkipper */
Resumen del diseño de escritorio {
    borde-radio: 100px !importante;
}
.layout-desktop fieldset.verticalSection-extrabottompadding,
.layout-tv fieldset.verticalSection-extrabottompadding {
    relleno: 10px 35px 20px 35px !importante;
}
#requisitos_introductorios,
#edl,
#silencio,
#apoyo {
    relleno inferior: 10px !importante;
}
/* Correcciones del panel de control para la versión 10.9.x */
.layout-desktop #userProfilesPage {
    izquierda: 260px !importante;
}
.MuiAlert-message {
    color: #fff !importante;
}
.MuiDataGrid-root.MuiDataGrid-withBorderColor {
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
.infoBanner {
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
.MuiToggleButton-root.MuiToggleButtonGroup-groupedHorizontal {
    borde-radio: var(--tarjetas-redondeadas);
    relleno en línea: 15px !important;
}
.MuiAppBar-root.MuiAppBar-positionFixed {
    relleno: 10px !importante;
}
.MuiAppBar-root.MuiAppBar-positionFixed.MuiAppBar-colorPrimary {
    fondo: var(--primary-background-transparent) !important;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.MuiList-root.MuiList-subencabezado {
    relleno izquierdo: 10px !important;
}
.MuiList-subheader .MuiListItem-root.MuiListItem-gutters {
    ancho: 85% !importante;
    margen-en-línea: auto !importante;
}
/* Corrección para la sección de plugins del panel de control */
[aria-labelledby="plugins-subheader"].MuiList-subheader .MuiListItemButton-root.MuiListItemButton-gutters {
    ancho: 85% !importante;
    margen-en-línea: auto !importante;
}
.MuiList-subheader .MuiListItemButton-root.MuiListItemButton-gutters {
    borde-radio: 100px !importante;
    margen: 2px 0px !importante;
    transición: .2s !importante;
    altura: 45px !importante
}
.MuiList-subheader .MuiListItemButton-root.MuiListItemButton-gutters:not(.Mui-selected) .MuiListItemIcon-root,
.MuiList-subheader .MuiListItemButton-root.MuiListItemButton-gutters:not(.Mui-selected) {
    color: #D1D1D1
}
.MuiList-subheader .MuiListItemButton-root.MuiListItemButton-gutters:hover:not(.Mui-selected) {
    transformar: escala(1.05) !importante;
    fondo: rgba(44, 44, 44, 0.7) !importante;
}
.MuiListItemButton-root.Mui-seleccionado {
    fondo: var(--color-de-acento-secundario) !importante;
}
.MuiListItemButton-root.Mui-selected .MuiListItemIcon-root,
.MuiListItemButton-root.Mui-seleccionado {
    color: var(--color-de-acento-primario) !importante;
}
.MuiPaper-root.MuiDrawer-paperAnchorDockedLeft {
    borde-derecha: ninguno !importante;
    fondo: var(--color-de-fondo-secundario) !importante;
    ancho: 250px !importante;
}
.MuiListItemIcon-root.MuiSvgIcon-fontSizeMedium {
    color: heredar !importante;
}
.MuiPaper-root.MuiPopover-paper {
    fondo: #252525 !importante;
    color: #D1D1D1 !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
.listItemIcon:not(.listItemIcon-transparent):not(.notification_important) {
    fondo: var(--color-de-acento-secundario) !importante;
    color: var(--color-de-acento-primario) !importante;
}
.MuiList-root:not(.MuiList-subheader) .MuiListItemButton-root.MuiListItemButton-gutters {
    relleno: 20px 38px 10px 38px !importante;
}
.MuiCollapse-root.MuiCollapse-vertical .MuiListItemButton-root.MuiListItemButton-gutters {
    ancho: 85% !importante;
    margen-en-línea: auto !importante;
    relleno: 8px 16px !importante;
}
/* Colores dinámicos para la sección "Dispositivos activos" para respetar el tema */
.defaultCardBackground1 {
    background-color: var(--primary-alt1) !important;
}
.defaultCardBackground2 {
    background-color: var(--primary-alt2) !important;
}
.defaultCardBackground3 {
    background-color: var(--primary-alt3) !important;
}
.defaultCardBackground4 {
    background-color: var(--primary-alt4) !important;
}
.defaultCardBackground5 {
    background-color: var(--primary-alt5) !important;
}
/* Modificar el relleno de los elementos del área de texto para que no se recorte la parte inferior */
área de texto {
    relleno inferior: 10px !importante;
}
/* Fondo detrás de los botones de navegación desplegables del panel de control */
@supports selector(:has(*)) {
    .MuiListItem-root:has(.MuiSvgIcon-root[data-testid^="Expandir"])::antes {
        contenido: '';
        posición: absoluta;
        fondo: #121212;
        margen: 1px -5px 0px -5px;
        borde-radio: 25px;
        opacidad: 0;
        transición: inserción 0,25 s, suavizado de salida, opacidad 0,01 s 0,25 s;
    }
    .MuiListItem-root:has(.MuiSvgIcon-root[data-testid="ExpandLessIcon"])::antes de {
        margen: 0px -5px -190px -5px;
        opacidad: 1;
        transición: inserción 0,25 s, suavizado de salida, opacidad 0,01 s;
    }
    .MuiListItemButton-root:has(.MuiSvgIcon-root[data-testid="ExpandLessIcon"]) {
        transformar: escala(1.05) !importante;
    }
    .MuiCollapse-raíz.MuiCollapse-vertical.MuiCollapse-entrada {
        relleno inferior: 5px !importante;
    }
}



/* Correcciones del editor de metadatos */
.layout-desktop .editPageSidebar {
    ancho: 25vw !importante;
}
.layout-desktop .editPageInnerContent {
    ancho: 74vw !importante;
}
.jstree-default-large .jstree-node {
    altura de línea: 35px !importante;
}
.jstree-default .jstree-wholerow-clicked {
    fondo: var(--color-de-acento-secundario) !importante;
}
.jstree-wholerow-hovered {
    fondo: var(--primary-background-transparent) !important;
}
.jstree-children {
    margen-izquierdo: -10px !importante;
}
#editItemMetadataPage .btnHeaderSave {
    fondo: var(--color-de-acento-primario) !importante;
    borde-radio: 100px !importante;
    altura: 40px !importante;
    color: blanco !importante;
}



/* Redimensionar la imagen del programa/película en la página de detalles */
.layout-desktop .detailImageContainer .card {
    arriba: 1.8em !importante;
    ancho: 18.3vw !importante;
    posición: ¡absoluta!importante;
}
/* Estilo heredado para no romper la compatibilidad con versiones anteriores a la 10.11.X */
.layout-desktop .infoWrapper .detailImageContainer .card {
    arriba: 9em !importante;
}

/* Reposicionar el contenido en la página de detalles */
.layout-desktop .detailSection {
    margen-derecho: 0 !importante;
}
.layout-desktop .detailPageContent {
    relleno-izquierda: 3.3% !importante;
    relleno-derecha: 0 !importante;
}

/* Reposicionar el logotipo */
.layout-desktop .detailLogo,
.layout-tv .detailLogo {
    derecha: 0 !importante;
    izquierda: 4% !importante;
    superior: 10% !importante;
}

/* Barra de cinta transparente */
.detailRibbon {
    fondo: transparente !importante;
}

/* Agregar tarjeta alrededor de los botones superiores derechos */
.mainDetailButtons {
    fondo: var(--primary-background-transparent) !important;
    borde-radio: 100px !importante;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}

/* Agregar tarjeta alrededor de la sección de grupos */
.layout-desktop .detailsGroupItem {
    fondo: var(--color-de-fondo-secundario) !importante;
    relleno: 10px 20px !importante;
    borde-radio: 20px !importante;
    ancho: ajustar-contenido !importante;
    ancho-máximo: contenido-máximo !importante;
    pantalla: flexible;
    espacio: 1em;
}

/* Corrección para las etiquetas de sección de grupo */
.detailsGroupItem .label, .trackSelections .selectContainer .selectLabel {
    ancho mínimo: 75px;
    flex-basis: no definido;
    margen: sin definir;
}

/* Tarjeta de sección de grupo móvil alternativa */
.layout-mobile .itemDetailsGroup {
    fondo: var(--color-de-fondo-secundario) !importante;
    relleno: 15px 20px 5px 20px !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
}
.layout-mobile .detailPageContent {
    relleno-derecha: 0 !importante;
}

/* Agregar tarjeta alrededor de la descripción */
.layout-desktop .detailSectionContent {
    fondo: var(--color-de-fondo-secundario) !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
    relleno: 40px 20px 10px 20px !importante;
    margen superior: 50px !importante;
}
@supports selector(:has(*)) {
    .layout-desktop .detailPageWrapperContainer:not(:has(.itemMiscInfo-primary .mediaInfoItem)) .detailSectionContent {
        relleno: 0px 20px 10px 20px !importante;
    }
}
.layout-mobile .detailSectionContent {
    fondo: var(--color-de-fondo-secundario) !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
    relleno: 10px 20px !importante;
}

/* Agregar tarjeta alrededor de la selección de pista */
.trackSelections {
    fondo: var(--color-de-fondo-secundario) !importante;
    borde-radio: var(--tarjetas-redondeadas) !importante;
    relleno: 10px 20px !importante;
    margen superior: 20px !importante;
}

/* Corrección para los menús desplegables de selección de pista */
.trackSelections .selectContainer .detailTrackSelect {
    relleno: 0 10px;
    margen izquierdo: 10px !importante;
}

/* Reposicionar título */
.layout-desktop .infoWrapper {
    margen superior: 245px !importante;
    margen-izquierda: 20.8vw !importante;
}
.layout-desktop .detailPagePrimaryContainer {
    relleno-izquierda: 3.3% !importante;
}
/* Corrección de la posición del título en 10.11.X */
.layout-desktop [dir="ltr"] .detailPagePrimaryContainer:not(.detailRibbon) .detailRibbon {
    relleno-izquierda: no definido !importante;
}
.layout-desktop .nameContainer {
    posición: ¡absoluta!importante;
    margen superior: -48px !importante;
}
.layout-desktop .itemMiscInfo {
    posición: ¡absoluta!importante;
    margen izquierdo: 12px !importante;
    margen superior: 16px !importante;
}

/* Mover el cuadro de descripción */
.layout-desktop .detailPagePrimaryContent {
    relleno-izquierda: 20.4vw !importante;
}
.layout-mobile .detailPagePrimaryContent {
    relleno-derecha: 5% !importante;
}
/* Espaciado para pósteres 2:3 */
.layout-desktop .detailPageWrapperContainer:has(.detailImageContainer .portraitCard) .detailPagePrimaryContent {
    altura mínima: 29vw !importante;
}
/* Espaciado para pósteres 1:1 */
.layout-desktop .detailPageWrapperContainer:has(.detailImageContainer .squareCard) .detailPagePrimaryContent {
    altura mínima: 20vw !importante;
}
/* Espaciado para pósteres 16:9 */
.layout-desktop .detailPageWrapperContainer:has(.detailImageContainer .backdropCard) .detailPagePrimaryContent {
    altura mínima: 12vw !importante;
}
/* Corrección para JMP */
@supports not selector(:has(*)) {
    .layout-desktop .detailPageWrapperContainer .detailPagePrimaryContent {
        altura mínima: 29vw !importante;
    }
}

/* Mover el cuadro de selección de pista */
.detailSection {
    pantalla: -webkit-box;
    pantalla: -moz-box;
    pantalla: caja;
    -webkit-box-orient: vertical;
    -moz-box-orient: vertical;
    orientación de la caja: vertical;
}
.detailSection .detailSectionContent {
    -webkit-box-ordinal-group: 1;
    -moz-box-ordinal-group: 1;
    grupo ordinal de caja: 1;
}
.detailSection .recordingFields {
    -webkit-box-ordinal-group: 2;
    -moz-box-ordinal-group: 2;
    grupo ordinal de caja: 2;
}
.detailSection .trackSelections {
    -webkit-box-ordinal-group: 3;
    -moz-box-ordinal-group: 3;
    grupo ordinal de caja: 3;
}
.detailSection .itemDetailsGroup {
    -webkit-box-ordinal-group: 4;
    -moz-box-ordinal-group: 4;
    grupo ordinal de caja: 4;
}
/* Mover título del episodio */
.layout-desktop .nameContainer {
    pantalla: -webkit-box;
    pantalla: -moz-box;
    pantalla: caja;
    -webkit-box-orient: horizontal;
    -moz-box-orient: horizontal;
    orientación de la caja: horizontal;
}
.layout-desktop .nameContainer .parentName {
    -webkit-box-ordinal-group: 1;
    -moz-box-ordinal-group: 1;
    grupo ordinal de caja: 1;
}
.layout-desktop .nameContainer .itemName {
    -webkit-box-ordinal-group: 2;
    -moz-box-ordinal-group: 2;
    grupo ordinal de caja: 2;
}
/* Modificar la posición del título original / nombre del episodio */
.layout-desktop .nameContainer .itemName.originalTitle {
    margen: .5em 20px !importante;
}
.layout-desktop .nameContainer .itemName.infoText.subtitle {
    margen: .5em 20px !importante;
    relleno: 0px !importante;
}
/* Modificar botón de reproducción */
.layout-desktop .mainDetailButtons .btnPlay::after {
    contenido: "Reproducir" !importante;
}
.layout-desktop .mainDetailButtons .btnPlay {
    posición: relativa !importante;
    margen-derecho: -85px !importante;
    relleno derecho: 20px !important;
    derecha: 110px !importante;
    fondo: var(--color-de-acento-primario) !importante;
    borde-radio: 100px !importante;
    color: var(--secondary-background-color) !important;
}
.layout-desktop .mainDetailButtons .detailButton {
    -webkit-flex-direction: fila !important;
    dirección flexible: fila !importante;
}
/* Cambiar el recorte para las imágenes de los elementos de la lista */
.listItemImage {
    tamaño de fondo: contener !importante;
    borde-radio: var(--tarjetas-redondeadas);
}
/* Mueve el contenido hacia arriba si no hay imagen de fondo - Puede que lo solucione en algún momento; ahora mismo hace que la página salte mientras se carga
@supports selector(:has(*)) {
    .layout-desktop:not(:has(.backdropContainer .backdropImage)) #itemBackdrop {
        altura: 20vh !importante;
    }
}
*/



/* Televisión en directo */
/* Color de fondo modificado de las celdas guía activas */
.programCell-active {
    fondo: var(--color-de-fondo-secundario) !importante;
}
/* Botón de grabación reposicionado */
.camposdegrabación {
    margen: 5px 0 -7px 0 !importante;
}
.botónDeGrabación {
    altura: 40px !importante;
}
.icono de grabación {
    color: rojo !importante;
}
/* Eliminar texto superpuesto */
.itemMiscInfo.itemMiscInfo-secundario {
    margen izquierdo: 65px !importante;
}



/* Reproductor de música */
.layout-desktop .appfooter {
    margen izquierdo: 250px !importante;
}
.layout-desktop .appfooter .nowPlayingBarInfoContainer {
    margen izquierdo: 10px !importante;
}
.layout-desktop .volumeOsd {
    borde-radio: var(--tarjetas-redondeadas) !importante;
    fondo: var(--secondary-background-transparent) !important;
}
.layout-desktop .nameContainer .musicParentName {
    margen superior: 18px !importante;
    margen-derecho: 22px !importante;
}
.layout-desktop .appfooter .nowPlayingBar {
    margen superior: 20px !importante;
}
.layout-desktop .appfooter .nowPlayingBar .nowPlayingBarPositionContainer {
    arriba: -15px !importante;
}



/* Solución para problemas de escalado */
@media (width: 1600px) {
    .layout-desktop .headerRight {
        margen-inferior: 0 !importante;
    }
    .layout-desktop .emby-button-foreground {
        arriba: -4px !importante;
    }
}
@media (max-width: 1599px) {
    .layout-desktop .pageTitleWithLogo {
        margen izquierdo: 25px !importante;
    }
    .layout-desktop .headerTabs {
        margen superior: -65px !importante;
    }
    .layout-desktop .headerRight {
        margen-derecho: 15px !importante;
    }
    .layout-desktop .sectionTabs {
        ancho: auto !importante;
        alinear-yo: centro !importante;
    }
    .layout-desktop .emby-button-foreground {
        arriba: -2px !importante;
    }
}



/* Correcciones para el diseño de TV */
.layout-tv .sectionTabs {
    ancho: auto !importante;
}
.layout-tv .headerLeft {
    relleno: 5px !importante;
}



/* Página de inicio de sesión */
.layout-desktop #loginPage {
    pantalla: flexible;
    justificar-contenido: centro;
    alinear elementos: centro;
}
.layout-desktop #loginPage .padded-left.padded-right.padded-bottom-page.margin-auto-y {
    fondo: var(--color-de-fondo-secundario) !importante;
    ancho: 400px !importante;
    borde-radio: 25px !importante;
    relleno: 50px !importante;
}
/* Corregir el relleno si no está presente el aviso legal de inicio de sesión */
.layout-desktop #loginPage .padded-left.padded-right.padded-bottom-page.margin-auto-y:not(:has(.loginDisclaimer p)) {
    relleno inferior: 100px !importante;
}
/* Mover el botón de cancelar */
.layout-desktop #loginPage .manualLoginForm .btnCancel {
    posición: ¡absoluta!importante;
    Antecedentes: ninguno !importante;
    ancho: 100px !importante;
    margen-izquierdo: -10px !importante;
    margen superior: 70px !importante;
    alineación del texto: izquierda !importante;
}
/* Botón de cancelación de Mayús en JMP */
@supports not selector(:has(*)) {
    .layout-desktop #loginPage .manualLoginForm .btnCancel {
        margen superior: 115px !importante;
    }
}
.layout-desktop #loginPage .visualLoginForm {
    posición: relativa !importante;
    fondo: var(--color-de-fondo-secundario) !importante;
    índice z: 1000 !importante;
}
.layout-desktop #loginPage .btnForgotPassword {
    Antecedentes: ninguno !importante;
    font-weight: normal !important;
    ancho: 150px !importante;
    alineación del texto: derecha !importante;
    posición: ¡absoluta!importante;
    margen izquierdo: 255px !importante;
    margen superior: -195px !importante;
    tamaño de fuente: más pequeño !importante;
    color: rgba(255, 255, 255, 0.5) !important;
    índice z: 1 !importante;
}
.layout-desktop #loginPage .loginDisclaimerContainer {
    arriba: 130px !importante;
    posición: relativa !importante;
    izquierda: -50px !importante;
    ancho: 500px !importante;
    margen superior: -35px !importante;
}
.layout-desktop #loginPage .squareCard {
    ancho: 25% !importante;
    tamaño de fuente: más pequeño !importante;
}
@media (max-width: 100em) {
    .layout-desktop #loginPage .squareCard {
        ancho: 20% !importante;
    }
    .layout-desktop #loginPage .padded-left.padded-right.padded-bottom-page.margin-auto-y {
        ancho: 600px !importante;
    }
    .layout-desktop #loginPage .btnForgotPassword {
        margen izquierdo: 450px !importante;
    }
    .layout-desktop #loginPage .disclaimerContainer {
        ancho: 700px !importante;
    }
}
@media (max-width: 87.5em) {
    .layout-desktop #loginPage .squareCard {
        ancho: 20% !importante;
    }
}
@media (max-width: 75em) {
    .layout-desktop #loginPage .squareCard {
        ancho: 20% !importante;
    }
}
@media (max-width: 43.75em) {
    .layout-desktop #loginPage .squareCard {
        ancho: 20% !importante;
    }
}



/* Cuadro de diálogo */
.diálogo {
    color de fondo: var(--color de fondo secundario) !importante;
}
.actionSheetTitle {
    margen: 10px 20px !importante;
}



/* Soporte para fondos dinámicos */

/* Tarjetas translúcidas */
.layout-desktop #itemDetailPage:not(.noBackdropTransparency) .detailsGroupItem,
.layout-desktop #itemDetailPage:not(.noBackdropTransparency) .detailSectionContent,
.layout-desktop #itemDetailPage:not(.noBackdropTransparency) .trackSelections {
    fondo: var(--primary-background-transparent) !important;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}

/* Cajón transparente */
.layout-desktop .backgroundContainer.withBackdrop + div .mainDrawer {
    fondo: degradado lineal (hacia la derecha, #10101090, transparente) !importante;
}
.layout-desktop:has(#itemDetailPage.noBackdropTransparency) .mainDrawer {
    fondo: var(--color-de-fondo-secundario) !importante;
}
/* Corrección para JMP */
@supports not selector(:has(*)) {
    .layout-desktop .backgroundContainer.withBackdrop + div .mainDrawer {
        fondo: transparente !importante;
    }
    .layout-desktop #itemDetailPage.noBackdropTransparency::after {
        posición: fija;
        contenido: "";
        superior: 0;
        izquierda: 0;
        altura: 100%;
        ancho: 250px;
        fondo: var(--color-de-fondo-secundario);
    }
}

/* Botones borrosos */
.layout-desktop:has(.backgroundContainer.withBackdrop) .navMenuOption-selected {
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}
.layout-desktop:has(.backgroundContainer.withBackdrop) .navMenuOption:hover:not(.navMenuOption-selected) {
    fondo: var(--primary-background-transparent) !important;
    filtro de fondo: desenfoque(var(--desenfoque)) !importante;
}8
