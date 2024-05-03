# Comparing `tmp/dara_components-1.8.5-py3-none-any.whl.zip` & `tmp/dara_components-1.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3078014 bytes, number of entries: 86
+Zip file size: 3081755 bytes, number of entries: 86
 -rw-r--r--  2.0 unx      808 b- defN 80-Jan-01 00:00 dara/components/__init__.py
 -rw-r--r--  2.0 unx     3866 b- defN 80-Jan-01 00:00 dara/components/common/__init__.py
 -rw-r--r--  2.0 unx     9487 b- defN 80-Jan-01 00:00 dara/components/common/accordion.py
 -rw-r--r--  2.0 unx     2869 b- defN 80-Jan-01 00:00 dara/components/common/anchor.py
 -rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 dara/components/common/base_component.py
 -rw-r--r--  2.0 unx     1433 b- defN 80-Jan-01 00:00 dara/components/common/bullet_list.py
 -rw-r--r--  2.0 unx     4549 b- defN 80-Jan-01 00:00 dara/components/common/button.py
@@ -75,14 +75,14 @@
 -rw-r--r--  2.0 unx     4120 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/data_slicer_modal.py
 -rw-r--r--  2.0 unx     1616 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/extension/data_slicer_filter.py
 -rw-r--r--  2.0 unx     1345 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/extension/filter_status_button.py
 -rw-r--r--  2.0 unx     8656 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/core.py
 -rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/data_preview.py
 -rw-r--r--  2.0 unx     3313 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/plotting.py
 -rw-r--r--  2.0 unx     2877 b- defN 80-Jan-01 00:00 dara/components/smart/hierarchy.py
--rw-r--r--  2.0 unx 16985599 b- defN 80-Jan-01 00:00 dara/components/umd/dara.components.umd.js
+-rw-r--r--  2.0 unx 17002704 b- defN 80-Jan-01 00:00 dara/components/umd/dara.components.umd.js
 -rw-r--r--  2.0 unx    23576 b- defN 80-Jan-01 00:00 dara/components/umd/style.css
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.8.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2710 b- defN 80-Jan-01 00:00 dara_components-1.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.8.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     8152 b- defN 16-Jan-01 00:00 dara_components-1.8.5.dist-info/RECORD
-86 files, 17315261 bytes uncompressed, 3064840 bytes compressed:  82.3%
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.8.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2710 b- defN 80-Jan-01 00:00 dara_components-1.8.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.8.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     8152 b- defN 16-Jan-01 00:00 dara_components-1.8.6.dist-info/RECORD
+86 files, 17332366 bytes uncompressed, 3068581 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -240,20 +240,20 @@
 
 Filename: dara/components/umd/dara.components.umd.js
 Comment: 
 
 Filename: dara/components/umd/style.css
 Comment: 
 
-Filename: dara_components-1.8.5.dist-info/LICENSE
+Filename: dara_components-1.8.6.dist-info/LICENSE
 Comment: 
 
-Filename: dara_components-1.8.5.dist-info/METADATA
+Filename: dara_components-1.8.6.dist-info/METADATA
 Comment: 
 
-Filename: dara_components-1.8.5.dist-info/WHEEL
+Filename: dara_components-1.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: dara_components-1.8.5.dist-info/RECORD
+Filename: dara_components-1.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dara/components/umd/dara.components.umd.js

### js-beautify {}

```diff
@@ -2552,24 +2552,24 @@
         mark: noop$1$1,
         measure: noop$1$1
     };
     var preamble = 'FA "6.4.2"';
     var begin = function begin2(name2) {
         p$3.mark("".concat(preamble, " ").concat(name2, " begins"));
         return function() {
-            return end$2(name2);
+            return end$1(name2);
         };
     };
-    var end$2 = function end2(name2) {
+    var end$1 = function end2(name2) {
         p$3.mark("".concat(preamble, " ").concat(name2, " ends"));
         p$3.measure("".concat(preamble, " ").concat(name2), "".concat(preamble, " ").concat(name2, " begins"), "".concat(preamble, " ").concat(name2, " ends"));
     };
     var perf = {
         begin,
-        end: end$2
+        end: end$1
     };
     var noop$2$1 = function noop2() {};
 
     function isWatched(node2) {
         var i2svg = node2.getAttribute ? node2.getAttribute(DATA_FA_I2SVG) : null;
         return typeof i2svg === "string";
     }
@@ -3761,16 +3761,16 @@
                     var symbol = symbolData === null ? false : symbolData === "" ? true : symbolData;
                     accumulator["symbol"] = symbol;
                     return accumulator;
                 }
             };
         }
     };
-    var plugins$1 = [InjectCSS, ReplaceElements, Layers, LayersCounter, LayersText, PseudoElements, MutationObserver$1, PowerTransforms, Masks, MissingIconIndicator, SvgSymbols];
-    registerPlugins(plugins$1, {
+    var plugins$2 = [InjectCSS, ReplaceElements, Layers, LayersCounter, LayersText, PseudoElements, MutationObserver$1, PowerTransforms, Masks, MissingIconIndicator, SvgSymbols];
+    registerPlugins(plugins$2, {
         mixoutsTo: api$1
     });
     api$1.noAuto;
     api$1.config;
     api$1.library;
     api$1.dom;
     var parse$1$1 = api$1.parse;
@@ -4777,30 +4777,14 @@
         background-color: ${(props) => props.theme.colors.primary};
     }
 
     &:last-child {
         border-bottom: none;
     }
 `;
-    const sameWidthModifier = {
-        effect: ({
-            state
-        }) => () => {
-            state.elements.popper.style.width = `${state.elements.reference.offsetWidth}px`;
-        },
-        enabled: true,
-        fn: ({
-            state
-        }) => {
-            state.styles.popper.width = `${state.rects.reference.width}px`;
-        },
-        name: "sameWidth",
-        phase: "beforeWrite",
-        requires: ["computeStyles"]
-    };
     globalThis && globalThis.__awaiter || function(thisArg, _arguments, P2, generator) {
         function adopt(value) {
             return value instanceof P2 ? value : new P2(function(resolve2) {
                 resolve2(value);
             });
         }
         return new(P2 || (P2 = Promise))(function(resolve2, reject) {
@@ -6298,15 +6282,15 @@
         isSymbol$3 = isSymbol_1$1;
     var NAN$1 = 0 / 0;
     var reIsBadHex$1 = /^[-+]0x[0-9a-f]+$/i;
     var reIsBinary$1 = /^0b[01]+$/i;
     var reIsOctal$1 = /^0o[0-7]+$/i;
     var freeParseInt$1 = parseInt;
 
-    function toNumber$5(value) {
+    function toNumber$4(value) {
         if (typeof value == "number") {
             return value;
         }
         if (isSymbol$3(value)) {
             return NAN$1;
         }
         if (isObject$7(value)) {
@@ -6316,35 +6300,35 @@
         if (typeof value != "string") {
             return value === 0 ? value : +value;
         }
         value = baseTrim$1(value);
         var isBinary = reIsBinary$1.test(value);
         return isBinary || reIsOctal$1.test(value) ? freeParseInt$1(value.slice(2), isBinary ? 2 : 8) : reIsBadHex$1.test(value) ? NAN$1 : +value;
     }
-    var toNumber_1$1 = toNumber$5;
+    var toNumber_1$1 = toNumber$4;
     var isObject$6 = isObject_1$1,
         now$3 = now_1$1,
-        toNumber$4 = toNumber_1$1;
+        toNumber$3 = toNumber_1$1;
     var FUNC_ERROR_TEXT$3 = "Expected a function";
     var nativeMax$1 = Math.max,
         nativeMin$2 = Math.min;
 
-    function debounce$7(func, wait, options) {
+    function debounce$6(func, wait, options) {
         var lastArgs, lastThis, maxWait, result, timerId, lastCallTime, lastInvokeTime = 0,
             leading = false,
             maxing = false,
             trailing = true;
         if (typeof func != "function") {
             throw new TypeError(FUNC_ERROR_TEXT$3);
         }
-        wait = toNumber$4(wait) || 0;
+        wait = toNumber$3(wait) || 0;
         if (isObject$6(options)) {
             leading = !!options.leading;
             maxing = "maxWait" in options;
-            maxWait = maxing ? nativeMax$1(toNumber$4(options.maxWait) || 0, wait) : maxWait;
+            maxWait = maxing ? nativeMax$1(toNumber$3(options.maxWait) || 0, wait) : maxWait;
             trailing = "trailing" in options ? !!options.trailing : trailing;
         }
 
         function invokeFunc(time) {
             var args = lastArgs,
                 thisArg = lastThis;
             lastArgs = lastThis = void 0;
@@ -6422,30 +6406,30 @@
             }
             return result;
         }
         debounced.cancel = cancel;
         debounced.flush = flush;
         return debounced;
     }
-    var debounce_1$1 = debounce$7;
-    var debounce$6 = debounce_1$1,
+    var debounce_1$1 = debounce$6;
+    var debounce$5 = debounce_1$1,
         isObject$5 = isObject_1$1;
     var FUNC_ERROR_TEXT$2 = "Expected a function";
 
     function throttle(func, wait, options) {
         var leading = true,
             trailing = true;
         if (typeof func != "function") {
             throw new TypeError(FUNC_ERROR_TEXT$2);
         }
         if (isObject$5(options)) {
             leading = "leading" in options ? !!options.leading : leading;
             trailing = "trailing" in options ? !!options.trailing : trailing;
         }
-        return debounce$6(func, wait, {
+        return debounce$5(func, wait, {
             "leading": leading,
             "maxWait": wait,
             "trailing": trailing
         });
     }
     var throttle_1 = throttle;
 
@@ -6677,14 +6661,2771 @@
         return {
             getItem,
             itemCount,
             onItemsRendered,
             refresh
         };
     }
+
+    function getNodeName$1(node2) {
+        if (isNode(node2)) {
+            return (node2.nodeName || "").toLowerCase();
+        }
+        return "#document";
+    }
+
+    function getWindow$1(node2) {
+        var _node$ownerDocument;
+        return (node2 == null || (_node$ownerDocument = node2.ownerDocument) == null ? void 0 : _node$ownerDocument.defaultView) || window;
+    }
+
+    function getDocumentElement$1(node2) {
+        var _ref2;
+        return (_ref2 = (isNode(node2) ? node2.ownerDocument : node2.document) || window.document) == null ? void 0 : _ref2.documentElement;
+    }
+
+    function isNode(value) {
+        return value instanceof Node || value instanceof getWindow$1(value).Node;
+    }
+
+    function isElement$4(value) {
+        return value instanceof Element || value instanceof getWindow$1(value).Element;
+    }
+
+    function isHTMLElement$1(value) {
+        return value instanceof HTMLElement || value instanceof getWindow$1(value).HTMLElement;
+    }
+
+    function isShadowRoot$1(value) {
+        if (typeof ShadowRoot === "undefined") {
+            return false;
+        }
+        return value instanceof ShadowRoot || value instanceof getWindow$1(value).ShadowRoot;
+    }
+
+    function isOverflowElement(element2) {
+        const {
+            overflow,
+            overflowX,
+            overflowY,
+            display
+        } = getComputedStyle$2(element2);
+        return /auto|scroll|overlay|hidden|clip/.test(overflow + overflowY + overflowX) && !["inline", "contents"].includes(display);
+    }
+
+    function isTableElement$1(element2) {
+        return ["table", "td", "th"].includes(getNodeName$1(element2));
+    }
+
+    function isContainingBlock(element2) {
+        const webkit2 = isWebKit();
+        const css2 = getComputedStyle$2(element2);
+        return css2.transform !== "none" || css2.perspective !== "none" || (css2.containerType ? css2.containerType !== "normal" : false) || !webkit2 && (css2.backdropFilter ? css2.backdropFilter !== "none" : false) || !webkit2 && (css2.filter ? css2.filter !== "none" : false) || ["transform", "perspective", "filter"].some((value) => (css2.willChange || "").includes(value)) || ["paint", "layout", "strict", "content"].some((value) => (css2.contain || "").includes(value));
+    }
+
+    function getContainingBlock$1(element2) {
+        let currentNode = getParentNode$1(element2);
+        while (isHTMLElement$1(currentNode) && !isLastTraversableNode(currentNode)) {
+            if (isContainingBlock(currentNode)) {
+                return currentNode;
+            }
+            currentNode = getParentNode$1(currentNode);
+        }
+        return null;
+    }
+
+    function isWebKit() {
+        if (typeof CSS === "undefined" || !CSS.supports)
+            return false;
+        return CSS.supports("-webkit-backdrop-filter", "none");
+    }
+
+    function isLastTraversableNode(node2) {
+        return ["html", "body", "#document"].includes(getNodeName$1(node2));
+    }
+
+    function getComputedStyle$2(element2) {
+        return getWindow$1(element2).getComputedStyle(element2);
+    }
+
+    function getNodeScroll$1(element2) {
+        if (isElement$4(element2)) {
+            return {
+                scrollLeft: element2.scrollLeft,
+                scrollTop: element2.scrollTop
+            };
+        }
+        return {
+            scrollLeft: element2.pageXOffset,
+            scrollTop: element2.pageYOffset
+        };
+    }
+
+    function getParentNode$1(node2) {
+        if (getNodeName$1(node2) === "html") {
+            return node2;
+        }
+        const result = node2.assignedSlot || node2.parentNode || isShadowRoot$1(node2) && node2.host || getDocumentElement$1(node2);
+        return isShadowRoot$1(result) ? result.host : result;
+    }
+
+    function getNearestOverflowAncestor(node2) {
+        const parentNode = getParentNode$1(node2);
+        if (isLastTraversableNode(parentNode)) {
+            return node2.ownerDocument ? node2.ownerDocument.body : node2.body;
+        }
+        if (isHTMLElement$1(parentNode) && isOverflowElement(parentNode)) {
+            return parentNode;
+        }
+        return getNearestOverflowAncestor(parentNode);
+    }
+
+    function getOverflowAncestors(node2, list2, traverseIframes) {
+        var _node$ownerDocument2;
+        if (list2 === void 0) {
+            list2 = [];
+        }
+        if (traverseIframes === void 0) {
+            traverseIframes = true;
+        }
+        const scrollableAncestor = getNearestOverflowAncestor(node2);
+        const isBody = scrollableAncestor === ((_node$ownerDocument2 = node2.ownerDocument) == null ? void 0 : _node$ownerDocument2.body);
+        const win = getWindow$1(scrollableAncestor);
+        if (isBody) {
+            return list2.concat(win, win.visualViewport || [], isOverflowElement(scrollableAncestor) ? scrollableAncestor : [], win.frameElement && traverseIframes ? getOverflowAncestors(win.frameElement) : []);
+        }
+        return list2.concat(scrollableAncestor, getOverflowAncestors(scrollableAncestor, [], traverseIframes));
+    }
+
+    function contains$2(parent, child) {
+        if (!parent || !child) {
+            return false;
+        }
+        const rootNode = child.getRootNode == null ? void 0 : child.getRootNode();
+        if (parent.contains(child)) {
+            return true;
+        }
+        if (rootNode && isShadowRoot$1(rootNode)) {
+            let next2 = child;
+            while (next2) {
+                if (parent === next2) {
+                    return true;
+                }
+                next2 = next2.parentNode || next2.host;
+            }
+        }
+        return false;
+    }
+
+    function isMouseLikePointerType(pointerType, strict) {
+        const values = ["mouse", "pen"];
+        if (!strict) {
+            values.push("", void 0);
+        }
+        return values.includes(pointerType);
+    }
+
+    function isReactEvent(event2) {
+        return "nativeEvent" in event2;
+    }
+
+    function isRootElement(element2) {
+        return element2.matches("html,body");
+    }
+
+    function getDocument(node2) {
+        return (node2 == null ? void 0 : node2.ownerDocument) || document;
+    }
+
+    function isEventTargetWithin(event2, node2) {
+        if (node2 == null) {
+            return false;
+        }
+        if ("composedPath" in event2) {
+            return event2.composedPath().includes(node2);
+        }
+        const e3 = event2;
+        return e3.target != null && node2.contains(e3.target);
+    }
+
+    function getTarget(event2) {
+        if ("composedPath" in event2) {
+            return event2.composedPath()[0];
+        }
+        return event2.target;
+    }
+    const TYPEABLE_SELECTOR = "input:not([type='hidden']):not([disabled]),[contenteditable]:not([contenteditable='false']),textarea:not([disabled])";
+
+    function isTypeableElement(element2) {
+        return isHTMLElement$1(element2) && element2.matches(TYPEABLE_SELECTOR);
+    }
+    const sides = ["top", "right", "bottom", "left"];
+    const alignments = ["start", "end"];
+    const placements$1 = /* @__PURE__ */ sides.reduce((acc, side) => acc.concat(side, side + "-" + alignments[0], side + "-" + alignments[1]), []);
+    const min$3 = Math.min;
+    const max$4 = Math.max;
+    const round$3 = Math.round;
+    const floor = Math.floor;
+    const createCoords = (v3) => ({
+        x: v3,
+        y: v3
+    });
+    const oppositeSideMap = {
+        left: "right",
+        right: "left",
+        bottom: "top",
+        top: "bottom"
+    };
+    const oppositeAlignmentMap = {
+        start: "end",
+        end: "start"
+    };
+
+    function clamp$1(start2, value, end2) {
+        return max$4(start2, min$3(value, end2));
+    }
+
+    function evaluate(value, param) {
+        return typeof value === "function" ? value(param) : value;
+    }
+
+    function getSide(placement) {
+        return placement.split("-")[0];
+    }
+
+    function getAlignment(placement) {
+        return placement.split("-")[1];
+    }
+
+    function getOppositeAxis(axis) {
+        return axis === "x" ? "y" : "x";
+    }
+
+    function getAxisLength(axis) {
+        return axis === "y" ? "height" : "width";
+    }
+
+    function getSideAxis(placement) {
+        return ["top", "bottom"].includes(getSide(placement)) ? "y" : "x";
+    }
+
+    function getAlignmentAxis(placement) {
+        return getOppositeAxis(getSideAxis(placement));
+    }
+
+    function getAlignmentSides(placement, rects, rtl) {
+        if (rtl === void 0) {
+            rtl = false;
+        }
+        const alignment = getAlignment(placement);
+        const alignmentAxis = getAlignmentAxis(placement);
+        const length = getAxisLength(alignmentAxis);
+        let mainAlignmentSide = alignmentAxis === "x" ? alignment === (rtl ? "end" : "start") ? "right" : "left" : alignment === "start" ? "bottom" : "top";
+        if (rects.reference[length] > rects.floating[length]) {
+            mainAlignmentSide = getOppositePlacement$1(mainAlignmentSide);
+        }
+        return [mainAlignmentSide, getOppositePlacement$1(mainAlignmentSide)];
+    }
+
+    function getExpandedPlacements(placement) {
+        const oppositePlacement = getOppositePlacement$1(placement);
+        return [getOppositeAlignmentPlacement(placement), oppositePlacement, getOppositeAlignmentPlacement(oppositePlacement)];
+    }
+
+    function getOppositeAlignmentPlacement(placement) {
+        return placement.replace(/start|end/g, (alignment) => oppositeAlignmentMap[alignment]);
+    }
+
+    function getSideList(side, isStart, rtl) {
+        const lr2 = ["left", "right"];
+        const rl = ["right", "left"];
+        const tb = ["top", "bottom"];
+        const bt2 = ["bottom", "top"];
+        switch (side) {
+            case "top":
+            case "bottom":
+                if (rtl)
+                    return isStart ? rl : lr2;
+                return isStart ? lr2 : rl;
+            case "left":
+            case "right":
+                return isStart ? tb : bt2;
+            default:
+                return [];
+        }
+    }
+
+    function getOppositeAxisPlacements(placement, flipAlignment, direction, rtl) {
+        const alignment = getAlignment(placement);
+        let list2 = getSideList(getSide(placement), direction === "start", rtl);
+        if (alignment) {
+            list2 = list2.map((side) => side + "-" + alignment);
+            if (flipAlignment) {
+                list2 = list2.concat(list2.map(getOppositeAlignmentPlacement));
+            }
+        }
+        return list2;
+    }
+
+    function getOppositePlacement$1(placement) {
+        return placement.replace(/left|right|bottom|top/g, (side) => oppositeSideMap[side]);
+    }
+
+    function expandPaddingObject(padding) {
+        return {
+            top: 0,
+            right: 0,
+            bottom: 0,
+            left: 0,
+            ...padding
+        };
+    }
+
+    function getPaddingObject(padding) {
+        return typeof padding !== "number" ? expandPaddingObject(padding) : {
+            top: padding,
+            right: padding,
+            bottom: padding,
+            left: padding
+        };
+    }
+
+    function rectToClientRect$1(rect) {
+        const {
+            x: x2,
+            y: y2,
+            width,
+            height
+        } = rect;
+        return {
+            width,
+            height,
+            top: y2,
+            left: x2,
+            right: x2 + width,
+            bottom: y2 + height,
+            x: x2,
+            y: y2
+        };
+    }
+
+    function computeCoordsFromPlacement(_ref2, placement, rtl) {
+        let {
+            reference: reference2,
+            floating
+        } = _ref2;
+        const sideAxis = getSideAxis(placement);
+        const alignmentAxis = getAlignmentAxis(placement);
+        const alignLength = getAxisLength(alignmentAxis);
+        const side = getSide(placement);
+        const isVertical = sideAxis === "y";
+        const commonX = reference2.x + reference2.width / 2 - floating.width / 2;
+        const commonY = reference2.y + reference2.height / 2 - floating.height / 2;
+        const commonAlign = reference2[alignLength] / 2 - floating[alignLength] / 2;
+        let coords;
+        switch (side) {
+            case "top":
+                coords = {
+                    x: commonX,
+                    y: reference2.y - floating.height
+                };
+                break;
+            case "bottom":
+                coords = {
+                    x: commonX,
+                    y: reference2.y + reference2.height
+                };
+                break;
+            case "right":
+                coords = {
+                    x: reference2.x + reference2.width,
+                    y: commonY
+                };
+                break;
+            case "left":
+                coords = {
+                    x: reference2.x - floating.width,
+                    y: commonY
+                };
+                break;
+            default:
+                coords = {
+                    x: reference2.x,
+                    y: reference2.y
+                };
+        }
+        switch (getAlignment(placement)) {
+            case "start":
+                coords[alignmentAxis] -= commonAlign * (rtl && isVertical ? -1 : 1);
+                break;
+            case "end":
+                coords[alignmentAxis] += commonAlign * (rtl && isVertical ? -1 : 1);
+                break;
+        }
+        return coords;
+    }
+    const computePosition$1 = async (reference2, floating, config2) => {
+        const {
+            placement = "bottom",
+                strategy = "absolute",
+                middleware = [],
+                platform: platform2
+        } = config2;
+        const validMiddleware = middleware.filter(Boolean);
+        const rtl = await (platform2.isRTL == null ? void 0 : platform2.isRTL(floating));
+        let rects = await platform2.getElementRects({
+            reference: reference2,
+            floating,
+            strategy
+        });
+        let {
+            x: x2,
+            y: y2
+        } = computeCoordsFromPlacement(rects, placement, rtl);
+        let statefulPlacement = placement;
+        let middlewareData = {};
+        let resetCount = 0;
+        for (let i2 = 0; i2 < validMiddleware.length; i2++) {
+            const {
+                name: name2,
+                fn: fn2
+            } = validMiddleware[i2];
+            const {
+                x: nextX,
+                y: nextY,
+                data: data2,
+                reset: reset2
+            } = await fn2({
+                x: x2,
+                y: y2,
+                initialPlacement: placement,
+                placement: statefulPlacement,
+                strategy,
+                middlewareData,
+                rects,
+                platform: platform2,
+                elements: {
+                    reference: reference2,
+                    floating
+                }
+            });
+            x2 = nextX != null ? nextX : x2;
+            y2 = nextY != null ? nextY : y2;
+            middlewareData = {
+                ...middlewareData,
+                [name2]: {
+                    ...middlewareData[name2],
+                    ...data2
+                }
+            };
+            if (reset2 && resetCount <= 50) {
+                resetCount++;
+                if (typeof reset2 === "object") {
+                    if (reset2.placement) {
+                        statefulPlacement = reset2.placement;
+                    }
+                    if (reset2.rects) {
+                        rects = reset2.rects === true ? await platform2.getElementRects({
+                            reference: reference2,
+                            floating,
+                            strategy
+                        }) : reset2.rects;
+                    }
+                    ({
+                        x: x2,
+                        y: y2
+                    } = computeCoordsFromPlacement(rects, statefulPlacement, rtl));
+                }
+                i2 = -1;
+            }
+        }
+        return {
+            x: x2,
+            y: y2,
+            placement: statefulPlacement,
+            strategy,
+            middlewareData
+        };
+    };
+    async function detectOverflow$1(state, options) {
+        var _await$platform$isEle;
+        if (options === void 0) {
+            options = {};
+        }
+        const {
+            x: x2,
+            y: y2,
+            platform: platform2,
+            rects,
+            elements,
+            strategy
+        } = state;
+        const {
+            boundary = "clippingAncestors",
+                rootBoundary = "viewport",
+                elementContext = "floating",
+                altBoundary = false,
+                padding = 0
+        } = evaluate(options, state);
+        const paddingObject = getPaddingObject(padding);
+        const altContext = elementContext === "floating" ? "reference" : "floating";
+        const element2 = elements[altBoundary ? altContext : elementContext];
+        const clippingClientRect = rectToClientRect$1(await platform2.getClippingRect({
+            element: ((_await$platform$isEle = await (platform2.isElement == null ? void 0 : platform2.isElement(element2))) != null ? _await$platform$isEle : true) ? element2 : element2.contextElement || await (platform2.getDocumentElement == null ? void 0 : platform2.getDocumentElement(elements.floating)),
+            boundary,
+            rootBoundary,
+            strategy
+        }));
+        const rect = elementContext === "floating" ? {
+            x: x2,
+            y: y2,
+            width: rects.floating.width,
+            height: rects.floating.height
+        } : rects.reference;
+        const offsetParent = await (platform2.getOffsetParent == null ? void 0 : platform2.getOffsetParent(elements.floating));
+        const offsetScale = await (platform2.isElement == null ? void 0 : platform2.isElement(offsetParent)) ? await (platform2.getScale == null ? void 0 : platform2.getScale(offsetParent)) || {
+            x: 1,
+            y: 1
+        } : {
+            x: 1,
+            y: 1
+        };
+        const elementClientRect = rectToClientRect$1(platform2.convertOffsetParentRelativeRectToViewportRelativeRect ? await platform2.convertOffsetParentRelativeRectToViewportRelativeRect({
+            elements,
+            rect,
+            offsetParent,
+            strategy
+        }) : rect);
+        return {
+            top: (clippingClientRect.top - elementClientRect.top + paddingObject.top) / offsetScale.y,
+            bottom: (elementClientRect.bottom - clippingClientRect.bottom + paddingObject.bottom) / offsetScale.y,
+            left: (clippingClientRect.left - elementClientRect.left + paddingObject.left) / offsetScale.x,
+            right: (elementClientRect.right - clippingClientRect.right + paddingObject.right) / offsetScale.x
+        };
+    }
+    const arrow$2 = (options) => ({
+        name: "arrow",
+        options,
+        async fn(state) {
+            const {
+                x: x2,
+                y: y2,
+                placement,
+                rects,
+                platform: platform2,
+                elements,
+                middlewareData
+            } = state;
+            const {
+                element: element2,
+                padding = 0
+            } = evaluate(options, state) || {};
+            if (element2 == null) {
+                return {};
+            }
+            const paddingObject = getPaddingObject(padding);
+            const coords = {
+                x: x2,
+                y: y2
+            };
+            const axis = getAlignmentAxis(placement);
+            const length = getAxisLength(axis);
+            const arrowDimensions = await platform2.getDimensions(element2);
+            const isYAxis = axis === "y";
+            const minProp = isYAxis ? "top" : "left";
+            const maxProp = isYAxis ? "bottom" : "right";
+            const clientProp = isYAxis ? "clientHeight" : "clientWidth";
+            const endDiff = rects.reference[length] + rects.reference[axis] - coords[axis] - rects.floating[length];
+            const startDiff = coords[axis] - rects.reference[axis];
+            const arrowOffsetParent = await (platform2.getOffsetParent == null ? void 0 : platform2.getOffsetParent(element2));
+            let clientSize = arrowOffsetParent ? arrowOffsetParent[clientProp] : 0;
+            if (!clientSize || !await (platform2.isElement == null ? void 0 : platform2.isElement(arrowOffsetParent))) {
+                clientSize = elements.floating[clientProp] || rects.floating[length];
+            }
+            const centerToReference = endDiff / 2 - startDiff / 2;
+            const largestPossiblePadding = clientSize / 2 - arrowDimensions[length] / 2 - 1;
+            const minPadding = min$3(paddingObject[minProp], largestPossiblePadding);
+            const maxPadding = min$3(paddingObject[maxProp], largestPossiblePadding);
+            const min$12 = minPadding;
+            const max2 = clientSize - arrowDimensions[length] - maxPadding;
+            const center2 = clientSize / 2 - arrowDimensions[length] / 2 + centerToReference;
+            const offset2 = clamp$1(min$12, center2, max2);
+            const shouldAddOffset = !middlewareData.arrow && getAlignment(placement) != null && center2 !== offset2 && rects.reference[length] / 2 - (center2 < min$12 ? minPadding : maxPadding) - arrowDimensions[length] / 2 < 0;
+            const alignmentOffset = shouldAddOffset ? center2 < min$12 ? center2 - min$12 : center2 - max2 : 0;
+            return {
+                [axis]: coords[axis] + alignmentOffset,
+                data: {
+                    [axis]: offset2,
+                    centerOffset: center2 - offset2 - alignmentOffset,
+                    ...shouldAddOffset && {
+                        alignmentOffset
+                    }
+                },
+                reset: shouldAddOffset
+            };
+        }
+    });
+
+    function getPlacementList(alignment, autoAlignment, allowedPlacements) {
+        const allowedPlacementsSortedByAlignment = alignment ? [...allowedPlacements.filter((placement) => getAlignment(placement) === alignment), ...allowedPlacements.filter((placement) => getAlignment(placement) !== alignment)] : allowedPlacements.filter((placement) => getSide(placement) === placement);
+        return allowedPlacementsSortedByAlignment.filter((placement) => {
+            if (alignment) {
+                return getAlignment(placement) === alignment || (autoAlignment ? getOppositeAlignmentPlacement(placement) !== placement : false);
+            }
+            return true;
+        });
+    }
+    const autoPlacement = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            name: "autoPlacement",
+            options,
+            async fn(state) {
+                var _middlewareData$autoP, _middlewareData$autoP2, _placementsThatFitOnE;
+                const {
+                    rects,
+                    middlewareData,
+                    placement,
+                    platform: platform2,
+                    elements
+                } = state;
+                const {
+                    crossAxis = false,
+                        alignment,
+                        allowedPlacements = placements$1,
+                        autoAlignment = true,
+                        ...detectOverflowOptions
+                } = evaluate(options, state);
+                const placements$1$1 = alignment !== void 0 || allowedPlacements === placements$1 ? getPlacementList(alignment || null, autoAlignment, allowedPlacements) : allowedPlacements;
+                const overflow = await detectOverflow$1(state, detectOverflowOptions);
+                const currentIndex = ((_middlewareData$autoP = middlewareData.autoPlacement) == null ? void 0 : _middlewareData$autoP.index) || 0;
+                const currentPlacement = placements$1$1[currentIndex];
+                if (currentPlacement == null) {
+                    return {};
+                }
+                const alignmentSides = getAlignmentSides(currentPlacement, rects, await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating)));
+                if (placement !== currentPlacement) {
+                    return {
+                        reset: {
+                            placement: placements$1$1[0]
+                        }
+                    };
+                }
+                const currentOverflows = [overflow[getSide(currentPlacement)], overflow[alignmentSides[0]], overflow[alignmentSides[1]]];
+                const allOverflows = [...((_middlewareData$autoP2 = middlewareData.autoPlacement) == null ? void 0 : _middlewareData$autoP2.overflows) || [], {
+                    placement: currentPlacement,
+                    overflows: currentOverflows
+                }];
+                const nextPlacement = placements$1$1[currentIndex + 1];
+                if (nextPlacement) {
+                    return {
+                        data: {
+                            index: currentIndex + 1,
+                            overflows: allOverflows
+                        },
+                        reset: {
+                            placement: nextPlacement
+                        }
+                    };
+                }
+                const placementsSortedByMostSpace = allOverflows.map((d2) => {
+                    const alignment2 = getAlignment(d2.placement);
+                    return [d2.placement, alignment2 && crossAxis ? d2.overflows.slice(0, 2).reduce((acc, v3) => acc + v3, 0) : d2.overflows[0], d2.overflows];
+                }).sort((a2, b2) => a2[1] - b2[1]);
+                const placementsThatFitOnEachSide = placementsSortedByMostSpace.filter((d2) => d2[2].slice(
+                    0,
+                    getAlignment(d2[0]) ? 2 : 3
+                ).every((v3) => v3 <= 0));
+                const resetPlacement = ((_placementsThatFitOnE = placementsThatFitOnEachSide[0]) == null ? void 0 : _placementsThatFitOnE[0]) || placementsSortedByMostSpace[0][0];
+                if (resetPlacement !== placement) {
+                    return {
+                        data: {
+                            index: currentIndex + 1,
+                            overflows: allOverflows
+                        },
+                        reset: {
+                            placement: resetPlacement
+                        }
+                    };
+                }
+                return {};
+            }
+        };
+    };
+    const flip$3 = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            name: "flip",
+            options,
+            async fn(state) {
+                var _middlewareData$arrow, _middlewareData$flip;
+                const {
+                    placement,
+                    middlewareData,
+                    rects,
+                    initialPlacement,
+                    platform: platform2,
+                    elements
+                } = state;
+                const {
+                    mainAxis: checkMainAxis = true,
+                    crossAxis: checkCrossAxis = true,
+                    fallbackPlacements: specifiedFallbackPlacements,
+                    fallbackStrategy = "bestFit",
+                    fallbackAxisSideDirection = "none",
+                    flipAlignment = true,
+                    ...detectOverflowOptions
+                } = evaluate(options, state);
+                if ((_middlewareData$arrow = middlewareData.arrow) != null && _middlewareData$arrow.alignmentOffset) {
+                    return {};
+                }
+                const side = getSide(placement);
+                const isBasePlacement = getSide(initialPlacement) === initialPlacement;
+                const rtl = await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating));
+                const fallbackPlacements = specifiedFallbackPlacements || (isBasePlacement || !flipAlignment ? [getOppositePlacement$1(initialPlacement)] : getExpandedPlacements(initialPlacement));
+                if (!specifiedFallbackPlacements && fallbackAxisSideDirection !== "none") {
+                    fallbackPlacements.push(...getOppositeAxisPlacements(initialPlacement, flipAlignment, fallbackAxisSideDirection, rtl));
+                }
+                const placements2 = [initialPlacement, ...fallbackPlacements];
+                const overflow = await detectOverflow$1(state, detectOverflowOptions);
+                const overflows = [];
+                let overflowsData = ((_middlewareData$flip = middlewareData.flip) == null ? void 0 : _middlewareData$flip.overflows) || [];
+                if (checkMainAxis) {
+                    overflows.push(overflow[side]);
+                }
+                if (checkCrossAxis) {
+                    const sides2 = getAlignmentSides(placement, rects, rtl);
+                    overflows.push(overflow[sides2[0]], overflow[sides2[1]]);
+                }
+                overflowsData = [...overflowsData, {
+                    placement,
+                    overflows
+                }];
+                if (!overflows.every((side2) => side2 <= 0)) {
+                    var _middlewareData$flip2, _overflowsData$filter;
+                    const nextIndex = (((_middlewareData$flip2 = middlewareData.flip) == null ? void 0 : _middlewareData$flip2.index) || 0) + 1;
+                    const nextPlacement = placements2[nextIndex];
+                    if (nextPlacement) {
+                        return {
+                            data: {
+                                index: nextIndex,
+                                overflows: overflowsData
+                            },
+                            reset: {
+                                placement: nextPlacement
+                            }
+                        };
+                    }
+                    let resetPlacement = (_overflowsData$filter = overflowsData.filter((d2) => d2.overflows[0] <= 0).sort((a2, b2) => a2.overflows[1] - b2.overflows[1])[0]) == null ? void 0 : _overflowsData$filter.placement;
+                    if (!resetPlacement) {
+                        switch (fallbackStrategy) {
+                            case "bestFit": {
+                                var _overflowsData$map$so;
+                                const placement2 = (_overflowsData$map$so = overflowsData.map((d2) => [d2.placement, d2.overflows.filter((overflow2) => overflow2 > 0).reduce((acc, overflow2) => acc + overflow2, 0)]).sort((a2, b2) => a2[1] - b2[1])[0]) == null ? void 0 : _overflowsData$map$so[0];
+                                if (placement2) {
+                                    resetPlacement = placement2;
+                                }
+                                break;
+                            }
+                            case "initialPlacement":
+                                resetPlacement = initialPlacement;
+                                break;
+                        }
+                    }
+                    if (placement !== resetPlacement) {
+                        return {
+                            reset: {
+                                placement: resetPlacement
+                            }
+                        };
+                    }
+                }
+                return {};
+            }
+        };
+    };
+
+    function getSideOffsets$1(overflow, rect) {
+        return {
+            top: overflow.top - rect.height,
+            right: overflow.right - rect.width,
+            bottom: overflow.bottom - rect.height,
+            left: overflow.left - rect.width
+        };
+    }
+
+    function isAnySideFullyClipped$1(overflow) {
+        return sides.some((side) => overflow[side] >= 0);
+    }
+    const hide$2 = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            name: "hide",
+            options,
+            async fn(state) {
+                const {
+                    rects
+                } = state;
+                const {
+                    strategy = "referenceHidden",
+                        ...detectOverflowOptions
+                } = evaluate(options, state);
+                switch (strategy) {
+                    case "referenceHidden": {
+                        const overflow = await detectOverflow$1(state, {
+                            ...detectOverflowOptions,
+                            elementContext: "reference"
+                        });
+                        const offsets = getSideOffsets$1(overflow, rects.reference);
+                        return {
+                            data: {
+                                referenceHiddenOffsets: offsets,
+                                referenceHidden: isAnySideFullyClipped$1(offsets)
+                            }
+                        };
+                    }
+                    case "escaped": {
+                        const overflow = await detectOverflow$1(state, {
+                            ...detectOverflowOptions,
+                            altBoundary: true
+                        });
+                        const offsets = getSideOffsets$1(overflow, rects.floating);
+                        return {
+                            data: {
+                                escapedOffsets: offsets,
+                                escaped: isAnySideFullyClipped$1(offsets)
+                            }
+                        };
+                    }
+                    default: {
+                        return {};
+                    }
+                }
+            }
+        };
+    };
+
+    function getBoundingRect(rects) {
+        const minX = min$3(...rects.map((rect) => rect.left));
+        const minY = min$3(...rects.map((rect) => rect.top));
+        const maxX = max$4(...rects.map((rect) => rect.right));
+        const maxY = max$4(...rects.map((rect) => rect.bottom));
+        return {
+            x: minX,
+            y: minY,
+            width: maxX - minX,
+            height: maxY - minY
+        };
+    }
+
+    function getRectsByLine(rects) {
+        const sortedRects = rects.slice().sort((a2, b2) => a2.y - b2.y);
+        const groups = [];
+        let prevRect = null;
+        for (let i2 = 0; i2 < sortedRects.length; i2++) {
+            const rect = sortedRects[i2];
+            if (!prevRect || rect.y - prevRect.y > prevRect.height / 2) {
+                groups.push([rect]);
+            } else {
+                groups[groups.length - 1].push(rect);
+            }
+            prevRect = rect;
+        }
+        return groups.map((rect) => rectToClientRect$1(getBoundingRect(rect)));
+    }
+    const inline = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            name: "inline",
+            options,
+            async fn(state) {
+                const {
+                    placement,
+                    elements,
+                    rects,
+                    platform: platform2,
+                    strategy
+                } = state;
+                const {
+                    padding = 2,
+                        x: x2,
+                        y: y2
+                } = evaluate(options, state);
+                const nativeClientRects = Array.from(await (platform2.getClientRects == null ? void 0 : platform2.getClientRects(elements.reference)) || []);
+                const clientRects = getRectsByLine(nativeClientRects);
+                const fallback = rectToClientRect$1(getBoundingRect(nativeClientRects));
+                const paddingObject = getPaddingObject(padding);
+
+                function getBoundingClientRect2() {
+                    if (clientRects.length === 2 && clientRects[0].left > clientRects[1].right && x2 != null && y2 != null) {
+                        return clientRects.find((rect) => x2 > rect.left - paddingObject.left && x2 < rect.right + paddingObject.right && y2 > rect.top - paddingObject.top && y2 < rect.bottom + paddingObject.bottom) || fallback;
+                    }
+                    if (clientRects.length >= 2) {
+                        if (getSideAxis(placement) === "y") {
+                            const firstRect = clientRects[0];
+                            const lastRect = clientRects[clientRects.length - 1];
+                            const isTop = getSide(placement) === "top";
+                            const top3 = firstRect.top;
+                            const bottom3 = lastRect.bottom;
+                            const left3 = isTop ? firstRect.left : lastRect.left;
+                            const right3 = isTop ? firstRect.right : lastRect.right;
+                            const width2 = right3 - left3;
+                            const height2 = bottom3 - top3;
+                            return {
+                                top: top3,
+                                bottom: bottom3,
+                                left: left3,
+                                right: right3,
+                                width: width2,
+                                height: height2,
+                                x: left3,
+                                y: top3
+                            };
+                        }
+                        const isLeftSide = getSide(placement) === "left";
+                        const maxRight = max$4(...clientRects.map((rect) => rect.right));
+                        const minLeft = min$3(...clientRects.map((rect) => rect.left));
+                        const measureRects = clientRects.filter((rect) => isLeftSide ? rect.left === minLeft : rect.right === maxRight);
+                        const top2 = measureRects[0].top;
+                        const bottom2 = measureRects[measureRects.length - 1].bottom;
+                        const left2 = minLeft;
+                        const right2 = maxRight;
+                        const width = right2 - left2;
+                        const height = bottom2 - top2;
+                        return {
+                            top: top2,
+                            bottom: bottom2,
+                            left: left2,
+                            right: right2,
+                            width,
+                            height,
+                            x: left2,
+                            y: top2
+                        };
+                    }
+                    return fallback;
+                }
+                const resetRects = await platform2.getElementRects({
+                    reference: {
+                        getBoundingClientRect: getBoundingClientRect2
+                    },
+                    floating: elements.floating,
+                    strategy
+                });
+                if (rects.reference.x !== resetRects.reference.x || rects.reference.y !== resetRects.reference.y || rects.reference.width !== resetRects.reference.width || rects.reference.height !== resetRects.reference.height) {
+                    return {
+                        reset: {
+                            rects: resetRects
+                        }
+                    };
+                }
+                return {};
+            }
+        };
+    };
+    async function convertValueToCoords(state, options) {
+        const {
+            placement,
+            platform: platform2,
+            elements
+        } = state;
+        const rtl = await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating));
+        const side = getSide(placement);
+        const alignment = getAlignment(placement);
+        const isVertical = getSideAxis(placement) === "y";
+        const mainAxisMulti = ["left", "top"].includes(side) ? -1 : 1;
+        const crossAxisMulti = rtl && isVertical ? -1 : 1;
+        const rawValue = evaluate(options, state);
+        let {
+            mainAxis,
+            crossAxis,
+            alignmentAxis
+        } = typeof rawValue === "number" ? {
+            mainAxis: rawValue,
+            crossAxis: 0,
+            alignmentAxis: null
+        } : {
+            mainAxis: 0,
+            crossAxis: 0,
+            alignmentAxis: null,
+            ...rawValue
+        };
+        if (alignment && typeof alignmentAxis === "number") {
+            crossAxis = alignment === "end" ? alignmentAxis * -1 : alignmentAxis;
+        }
+        return isVertical ? {
+            x: crossAxis * crossAxisMulti,
+            y: mainAxis * mainAxisMulti
+        } : {
+            x: mainAxis * mainAxisMulti,
+            y: crossAxis * crossAxisMulti
+        };
+    }
+    const offset$3 = function(options) {
+        if (options === void 0) {
+            options = 0;
+        }
+        return {
+            name: "offset",
+            options,
+            async fn(state) {
+                var _middlewareData$offse, _middlewareData$arrow;
+                const {
+                    x: x2,
+                    y: y2,
+                    placement,
+                    middlewareData
+                } = state;
+                const diffCoords = await convertValueToCoords(state, options);
+                if (placement === ((_middlewareData$offse = middlewareData.offset) == null ? void 0 : _middlewareData$offse.placement) && (_middlewareData$arrow = middlewareData.arrow) != null && _middlewareData$arrow.alignmentOffset) {
+                    return {};
+                }
+                return {
+                    x: x2 + diffCoords.x,
+                    y: y2 + diffCoords.y,
+                    data: {
+                        ...diffCoords,
+                        placement
+                    }
+                };
+            }
+        };
+    };
+    const shift$2 = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            name: "shift",
+            options,
+            async fn(state) {
+                const {
+                    x: x2,
+                    y: y2,
+                    placement
+                } = state;
+                const {
+                    mainAxis: checkMainAxis = true,
+                    crossAxis: checkCrossAxis = false,
+                    limiter = {
+                        fn: (_ref2) => {
+                            let {
+                                x: x3,
+                                y: y3
+                            } = _ref2;
+                            return {
+                                x: x3,
+                                y: y3
+                            };
+                        }
+                    },
+                    ...detectOverflowOptions
+                } = evaluate(options, state);
+                const coords = {
+                    x: x2,
+                    y: y2
+                };
+                const overflow = await detectOverflow$1(state, detectOverflowOptions);
+                const crossAxis = getSideAxis(getSide(placement));
+                const mainAxis = getOppositeAxis(crossAxis);
+                let mainAxisCoord = coords[mainAxis];
+                let crossAxisCoord = coords[crossAxis];
+                if (checkMainAxis) {
+                    const minSide = mainAxis === "y" ? "top" : "left";
+                    const maxSide = mainAxis === "y" ? "bottom" : "right";
+                    const min2 = mainAxisCoord + overflow[minSide];
+                    const max2 = mainAxisCoord - overflow[maxSide];
+                    mainAxisCoord = clamp$1(min2, mainAxisCoord, max2);
+                }
+                if (checkCrossAxis) {
+                    const minSide = crossAxis === "y" ? "top" : "left";
+                    const maxSide = crossAxis === "y" ? "bottom" : "right";
+                    const min2 = crossAxisCoord + overflow[minSide];
+                    const max2 = crossAxisCoord - overflow[maxSide];
+                    crossAxisCoord = clamp$1(min2, crossAxisCoord, max2);
+                }
+                const limitedCoords = limiter.fn({
+                    ...state,
+                    [mainAxis]: mainAxisCoord,
+                    [crossAxis]: crossAxisCoord
+                });
+                return {
+                    ...limitedCoords,
+                    data: {
+                        x: limitedCoords.x - x2,
+                        y: limitedCoords.y - y2
+                    }
+                };
+            }
+        };
+    };
+    const limitShift = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            options,
+            fn(state) {
+                const {
+                    x: x2,
+                    y: y2,
+                    placement,
+                    rects,
+                    middlewareData
+                } = state;
+                const {
+                    offset: offset2 = 0,
+                    mainAxis: checkMainAxis = true,
+                    crossAxis: checkCrossAxis = true
+                } = evaluate(options, state);
+                const coords = {
+                    x: x2,
+                    y: y2
+                };
+                const crossAxis = getSideAxis(placement);
+                const mainAxis = getOppositeAxis(crossAxis);
+                let mainAxisCoord = coords[mainAxis];
+                let crossAxisCoord = coords[crossAxis];
+                const rawOffset = evaluate(offset2, state);
+                const computedOffset = typeof rawOffset === "number" ? {
+                    mainAxis: rawOffset,
+                    crossAxis: 0
+                } : {
+                    mainAxis: 0,
+                    crossAxis: 0,
+                    ...rawOffset
+                };
+                if (checkMainAxis) {
+                    const len = mainAxis === "y" ? "height" : "width";
+                    const limitMin = rects.reference[mainAxis] - rects.floating[len] + computedOffset.mainAxis;
+                    const limitMax = rects.reference[mainAxis] + rects.reference[len] - computedOffset.mainAxis;
+                    if (mainAxisCoord < limitMin) {
+                        mainAxisCoord = limitMin;
+                    } else if (mainAxisCoord > limitMax) {
+                        mainAxisCoord = limitMax;
+                    }
+                }
+                if (checkCrossAxis) {
+                    var _middlewareData$offse, _middlewareData$offse2;
+                    const len = mainAxis === "y" ? "width" : "height";
+                    const isOriginSide = ["top", "left"].includes(getSide(placement));
+                    const limitMin = rects.reference[crossAxis] - rects.floating[len] + (isOriginSide ? ((_middlewareData$offse = middlewareData.offset) == null ? void 0 : _middlewareData$offse[crossAxis]) || 0 : 0) + (isOriginSide ? 0 : computedOffset.crossAxis);
+                    const limitMax = rects.reference[crossAxis] + rects.reference[len] + (isOriginSide ? 0 : ((_middlewareData$offse2 = middlewareData.offset) == null ? void 0 : _middlewareData$offse2[crossAxis]) || 0) - (isOriginSide ? computedOffset.crossAxis : 0);
+                    if (crossAxisCoord < limitMin) {
+                        crossAxisCoord = limitMin;
+                    } else if (crossAxisCoord > limitMax) {
+                        crossAxisCoord = limitMax;
+                    }
+                }
+                return {
+                    [mainAxis]: mainAxisCoord,
+                    [crossAxis]: crossAxisCoord
+                };
+            }
+        };
+    };
+    const size$2 = function(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        return {
+            name: "size",
+            options,
+            async fn(state) {
+                const {
+                    placement,
+                    rects,
+                    platform: platform2,
+                    elements
+                } = state;
+                const {
+                    apply = () => {},
+                        ...detectOverflowOptions
+                } = evaluate(options, state);
+                const overflow = await detectOverflow$1(state, detectOverflowOptions);
+                const side = getSide(placement);
+                const alignment = getAlignment(placement);
+                const isYAxis = getSideAxis(placement) === "y";
+                const {
+                    width,
+                    height
+                } = rects.floating;
+                let heightSide;
+                let widthSide;
+                if (side === "top" || side === "bottom") {
+                    heightSide = side;
+                    widthSide = alignment === (await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating)) ? "start" : "end") ? "left" : "right";
+                } else {
+                    widthSide = side;
+                    heightSide = alignment === "end" ? "top" : "bottom";
+                }
+                const overflowAvailableHeight = height - overflow[heightSide];
+                const overflowAvailableWidth = width - overflow[widthSide];
+                const noShift = !state.middlewareData.shift;
+                let availableHeight = overflowAvailableHeight;
+                let availableWidth = overflowAvailableWidth;
+                if (isYAxis) {
+                    const maximumClippingWidth = width - overflow.left - overflow.right;
+                    availableWidth = alignment || noShift ? min$3(overflowAvailableWidth, maximumClippingWidth) : maximumClippingWidth;
+                } else {
+                    const maximumClippingHeight = height - overflow.top - overflow.bottom;
+                    availableHeight = alignment || noShift ? min$3(overflowAvailableHeight, maximumClippingHeight) : maximumClippingHeight;
+                }
+                if (noShift && !alignment) {
+                    const xMin = max$4(overflow.left, 0);
+                    const xMax = max$4(overflow.right, 0);
+                    const yMin = max$4(overflow.top, 0);
+                    const yMax = max$4(overflow.bottom, 0);
+                    if (isYAxis) {
+                        availableWidth = width - 2 * (xMin !== 0 || xMax !== 0 ? xMin + xMax : max$4(overflow.left, overflow.right));
+                    } else {
+                        availableHeight = height - 2 * (yMin !== 0 || yMax !== 0 ? yMin + yMax : max$4(overflow.top, overflow.bottom));
+                    }
+                }
+                await apply({
+                    ...state,
+                    availableWidth,
+                    availableHeight
+                });
+                const nextDimensions = await platform2.getDimensions(elements.floating);
+                if (width !== nextDimensions.width || height !== nextDimensions.height) {
+                    return {
+                        reset: {
+                            rects: true
+                        }
+                    };
+                }
+                return {};
+            }
+        };
+    };
+
+    function getCssDimensions(element2) {
+        const css2 = getComputedStyle$2(element2);
+        let width = parseFloat(css2.width) || 0;
+        let height = parseFloat(css2.height) || 0;
+        const hasOffset = isHTMLElement$1(element2);
+        const offsetWidth = hasOffset ? element2.offsetWidth : width;
+        const offsetHeight = hasOffset ? element2.offsetHeight : height;
+        const shouldFallback = round$3(width) !== offsetWidth || round$3(height) !== offsetHeight;
+        if (shouldFallback) {
+            width = offsetWidth;
+            height = offsetHeight;
+        }
+        return {
+            width,
+            height,
+            $: shouldFallback
+        };
+    }
+
+    function unwrapElement(element2) {
+        return !isElement$4(element2) ? element2.contextElement : element2;
+    }
+
+    function getScale$1(element2) {
+        const domElement2 = unwrapElement(element2);
+        if (!isHTMLElement$1(domElement2)) {
+            return createCoords(1);
+        }
+        const rect = domElement2.getBoundingClientRect();
+        const {
+            width,
+            height,
+            $: $2
+        } = getCssDimensions(domElement2);
+        let x2 = ($2 ? round$3(rect.width) : rect.width) / width;
+        let y2 = ($2 ? round$3(rect.height) : rect.height) / height;
+        if (!x2 || !Number.isFinite(x2)) {
+            x2 = 1;
+        }
+        if (!y2 || !Number.isFinite(y2)) {
+            y2 = 1;
+        }
+        return {
+            x: x2,
+            y: y2
+        };
+    }
+    const noOffsets = /* @__PURE__ */ createCoords(0);
+
+    function getVisualOffsets(element2) {
+        const win = getWindow$1(element2);
+        if (!isWebKit() || !win.visualViewport) {
+            return noOffsets;
+        }
+        return {
+            x: win.visualViewport.offsetLeft,
+            y: win.visualViewport.offsetTop
+        };
+    }
+
+    function shouldAddVisualOffsets(element2, isFixed, floatingOffsetParent) {
+        if (isFixed === void 0) {
+            isFixed = false;
+        }
+        if (!floatingOffsetParent || isFixed && floatingOffsetParent !== getWindow$1(element2)) {
+            return false;
+        }
+        return isFixed;
+    }
+
+    function getBoundingClientRect$1(element2, includeScale, isFixedStrategy, offsetParent) {
+        if (includeScale === void 0) {
+            includeScale = false;
+        }
+        if (isFixedStrategy === void 0) {
+            isFixedStrategy = false;
+        }
+        const clientRect = element2.getBoundingClientRect();
+        const domElement2 = unwrapElement(element2);
+        let scale = createCoords(1);
+        if (includeScale) {
+            if (offsetParent) {
+                if (isElement$4(offsetParent)) {
+                    scale = getScale$1(offsetParent);
+                }
+            } else {
+                scale = getScale$1(element2);
+            }
+        }
+        const visualOffsets = shouldAddVisualOffsets(domElement2, isFixedStrategy, offsetParent) ? getVisualOffsets(domElement2) : createCoords(0);
+        let x2 = (clientRect.left + visualOffsets.x) / scale.x;
+        let y2 = (clientRect.top + visualOffsets.y) / scale.y;
+        let width = clientRect.width / scale.x;
+        let height = clientRect.height / scale.y;
+        if (domElement2) {
+            const win = getWindow$1(domElement2);
+            const offsetWin = offsetParent && isElement$4(offsetParent) ? getWindow$1(offsetParent) : offsetParent;
+            let currentWin = win;
+            let currentIFrame = currentWin.frameElement;
+            while (currentIFrame && offsetParent && offsetWin !== currentWin) {
+                const iframeScale = getScale$1(currentIFrame);
+                const iframeRect = currentIFrame.getBoundingClientRect();
+                const css2 = getComputedStyle$2(currentIFrame);
+                const left2 = iframeRect.left + (currentIFrame.clientLeft + parseFloat(css2.paddingLeft)) * iframeScale.x;
+                const top2 = iframeRect.top + (currentIFrame.clientTop + parseFloat(css2.paddingTop)) * iframeScale.y;
+                x2 *= iframeScale.x;
+                y2 *= iframeScale.y;
+                width *= iframeScale.x;
+                height *= iframeScale.y;
+                x2 += left2;
+                y2 += top2;
+                currentWin = getWindow$1(currentIFrame);
+                currentIFrame = currentWin.frameElement;
+            }
+        }
+        return rectToClientRect$1({
+            width,
+            height,
+            x: x2,
+            y: y2
+        });
+    }
+    const topLayerSelectors = [":popover-open", ":modal"];
+
+    function isTopLayer(floating) {
+        return topLayerSelectors.some((selector2) => {
+            try {
+                return floating.matches(selector2);
+            } catch (e3) {
+                return false;
+            }
+        });
+    }
+
+    function convertOffsetParentRelativeRectToViewportRelativeRect(_ref2) {
+        let {
+            elements,
+            rect,
+            offsetParent,
+            strategy
+        } = _ref2;
+        const isFixed = strategy === "fixed";
+        const documentElement = getDocumentElement$1(offsetParent);
+        const topLayer = elements ? isTopLayer(elements.floating) : false;
+        if (offsetParent === documentElement || topLayer && isFixed) {
+            return rect;
+        }
+        let scroll = {
+            scrollLeft: 0,
+            scrollTop: 0
+        };
+        let scale = createCoords(1);
+        const offsets = createCoords(0);
+        const isOffsetParentAnElement = isHTMLElement$1(offsetParent);
+        if (isOffsetParentAnElement || !isOffsetParentAnElement && !isFixed) {
+            if (getNodeName$1(offsetParent) !== "body" || isOverflowElement(documentElement)) {
+                scroll = getNodeScroll$1(offsetParent);
+            }
+            if (isHTMLElement$1(offsetParent)) {
+                const offsetRect = getBoundingClientRect$1(offsetParent);
+                scale = getScale$1(offsetParent);
+                offsets.x = offsetRect.x + offsetParent.clientLeft;
+                offsets.y = offsetRect.y + offsetParent.clientTop;
+            }
+        }
+        return {
+            width: rect.width * scale.x,
+            height: rect.height * scale.y,
+            x: rect.x * scale.x - scroll.scrollLeft * scale.x + offsets.x,
+            y: rect.y * scale.y - scroll.scrollTop * scale.y + offsets.y
+        };
+    }
+
+    function getClientRects(element2) {
+        return Array.from(element2.getClientRects());
+    }
+
+    function getWindowScrollBarX$1(element2) {
+        return getBoundingClientRect$1(getDocumentElement$1(element2)).left + getNodeScroll$1(element2).scrollLeft;
+    }
+
+    function getDocumentRect$1(element2) {
+        const html2 = getDocumentElement$1(element2);
+        const scroll = getNodeScroll$1(element2);
+        const body = element2.ownerDocument.body;
+        const width = max$4(html2.scrollWidth, html2.clientWidth, body.scrollWidth, body.clientWidth);
+        const height = max$4(html2.scrollHeight, html2.clientHeight, body.scrollHeight, body.clientHeight);
+        let x2 = -scroll.scrollLeft + getWindowScrollBarX$1(element2);
+        const y2 = -scroll.scrollTop;
+        if (getComputedStyle$2(body).direction === "rtl") {
+            x2 += max$4(html2.clientWidth, body.clientWidth) - width;
+        }
+        return {
+            width,
+            height,
+            x: x2,
+            y: y2
+        };
+    }
+
+    function getViewportRect$1(element2, strategy) {
+        const win = getWindow$1(element2);
+        const html2 = getDocumentElement$1(element2);
+        const visualViewport = win.visualViewport;
+        let width = html2.clientWidth;
+        let height = html2.clientHeight;
+        let x2 = 0;
+        let y2 = 0;
+        if (visualViewport) {
+            width = visualViewport.width;
+            height = visualViewport.height;
+            const visualViewportBased = isWebKit();
+            if (!visualViewportBased || visualViewportBased && strategy === "fixed") {
+                x2 = visualViewport.offsetLeft;
+                y2 = visualViewport.offsetTop;
+            }
+        }
+        return {
+            width,
+            height,
+            x: x2,
+            y: y2
+        };
+    }
+
+    function getInnerBoundingClientRect$1(element2, strategy) {
+        const clientRect = getBoundingClientRect$1(element2, true, strategy === "fixed");
+        const top2 = clientRect.top + element2.clientTop;
+        const left2 = clientRect.left + element2.clientLeft;
+        const scale = isHTMLElement$1(element2) ? getScale$1(element2) : createCoords(1);
+        const width = element2.clientWidth * scale.x;
+        const height = element2.clientHeight * scale.y;
+        const x2 = left2 * scale.x;
+        const y2 = top2 * scale.y;
+        return {
+            width,
+            height,
+            x: x2,
+            y: y2
+        };
+    }
+
+    function getClientRectFromClippingAncestor(element2, clippingAncestor, strategy) {
+        let rect;
+        if (clippingAncestor === "viewport") {
+            rect = getViewportRect$1(element2, strategy);
+        } else if (clippingAncestor === "document") {
+            rect = getDocumentRect$1(getDocumentElement$1(element2));
+        } else if (isElement$4(clippingAncestor)) {
+            rect = getInnerBoundingClientRect$1(clippingAncestor, strategy);
+        } else {
+            const visualOffsets = getVisualOffsets(element2);
+            rect = {
+                ...clippingAncestor,
+                x: clippingAncestor.x - visualOffsets.x,
+                y: clippingAncestor.y - visualOffsets.y
+            };
+        }
+        return rectToClientRect$1(rect);
+    }
+
+    function hasFixedPositionAncestor(element2, stopNode) {
+        const parentNode = getParentNode$1(element2);
+        if (parentNode === stopNode || !isElement$4(parentNode) || isLastTraversableNode(parentNode)) {
+            return false;
+        }
+        return getComputedStyle$2(parentNode).position === "fixed" || hasFixedPositionAncestor(parentNode, stopNode);
+    }
+
+    function getClippingElementAncestors(element2, cache2) {
+        const cachedResult = cache2.get(element2);
+        if (cachedResult) {
+            return cachedResult;
+        }
+        let result = getOverflowAncestors(element2, [], false).filter((el) => isElement$4(el) && getNodeName$1(el) !== "body");
+        let currentContainingBlockComputedStyle = null;
+        const elementIsFixed = getComputedStyle$2(element2).position === "fixed";
+        let currentNode = elementIsFixed ? getParentNode$1(element2) : element2;
+        while (isElement$4(currentNode) && !isLastTraversableNode(currentNode)) {
+            const computedStyle = getComputedStyle$2(currentNode);
+            const currentNodeIsContaining = isContainingBlock(currentNode);
+            if (!currentNodeIsContaining && computedStyle.position === "fixed") {
+                currentContainingBlockComputedStyle = null;
+            }
+            const shouldDropCurrentNode = elementIsFixed ? !currentNodeIsContaining && !currentContainingBlockComputedStyle : !currentNodeIsContaining && computedStyle.position === "static" && !!currentContainingBlockComputedStyle && ["absolute", "fixed"].includes(currentContainingBlockComputedStyle.position) || isOverflowElement(currentNode) && !currentNodeIsContaining && hasFixedPositionAncestor(element2, currentNode);
+            if (shouldDropCurrentNode) {
+                result = result.filter((ancestor) => ancestor !== currentNode);
+            } else {
+                currentContainingBlockComputedStyle = computedStyle;
+            }
+            currentNode = getParentNode$1(currentNode);
+        }
+        cache2.set(element2, result);
+        return result;
+    }
+
+    function getClippingRect$1(_ref2) {
+        let {
+            element: element2,
+            boundary,
+            rootBoundary,
+            strategy
+        } = _ref2;
+        const elementClippingAncestors = boundary === "clippingAncestors" ? getClippingElementAncestors(element2, this._c) : [].concat(boundary);
+        const clippingAncestors = [...elementClippingAncestors, rootBoundary];
+        const firstClippingAncestor = clippingAncestors[0];
+        const clippingRect = clippingAncestors.reduce((accRect, clippingAncestor) => {
+            const rect = getClientRectFromClippingAncestor(element2, clippingAncestor, strategy);
+            accRect.top = max$4(rect.top, accRect.top);
+            accRect.right = min$3(rect.right, accRect.right);
+            accRect.bottom = min$3(rect.bottom, accRect.bottom);
+            accRect.left = max$4(rect.left, accRect.left);
+            return accRect;
+        }, getClientRectFromClippingAncestor(element2, firstClippingAncestor, strategy));
+        return {
+            width: clippingRect.right - clippingRect.left,
+            height: clippingRect.bottom - clippingRect.top,
+            x: clippingRect.left,
+            y: clippingRect.top
+        };
+    }
+
+    function getDimensions(element2) {
+        const {
+            width,
+            height
+        } = getCssDimensions(element2);
+        return {
+            width,
+            height
+        };
+    }
+
+    function getRectRelativeToOffsetParent(element2, offsetParent, strategy) {
+        const isOffsetParentAnElement = isHTMLElement$1(offsetParent);
+        const documentElement = getDocumentElement$1(offsetParent);
+        const isFixed = strategy === "fixed";
+        const rect = getBoundingClientRect$1(element2, true, isFixed, offsetParent);
+        let scroll = {
+            scrollLeft: 0,
+            scrollTop: 0
+        };
+        const offsets = createCoords(0);
+        if (isOffsetParentAnElement || !isOffsetParentAnElement && !isFixed) {
+            if (getNodeName$1(offsetParent) !== "body" || isOverflowElement(documentElement)) {
+                scroll = getNodeScroll$1(offsetParent);
+            }
+            if (isOffsetParentAnElement) {
+                const offsetRect = getBoundingClientRect$1(offsetParent, true, isFixed, offsetParent);
+                offsets.x = offsetRect.x + offsetParent.clientLeft;
+                offsets.y = offsetRect.y + offsetParent.clientTop;
+            } else if (documentElement) {
+                offsets.x = getWindowScrollBarX$1(documentElement);
+            }
+        }
+        const x2 = rect.left + scroll.scrollLeft - offsets.x;
+        const y2 = rect.top + scroll.scrollTop - offsets.y;
+        return {
+            x: x2,
+            y: y2,
+            width: rect.width,
+            height: rect.height
+        };
+    }
+
+    function getTrueOffsetParent$1(element2, polyfill) {
+        if (!isHTMLElement$1(element2) || getComputedStyle$2(element2).position === "fixed") {
+            return null;
+        }
+        if (polyfill) {
+            return polyfill(element2);
+        }
+        return element2.offsetParent;
+    }
+
+    function getOffsetParent$1(element2, polyfill) {
+        const window2 = getWindow$1(element2);
+        if (!isHTMLElement$1(element2) || isTopLayer(element2)) {
+            return window2;
+        }
+        let offsetParent = getTrueOffsetParent$1(element2, polyfill);
+        while (offsetParent && isTableElement$1(offsetParent) && getComputedStyle$2(offsetParent).position === "static") {
+            offsetParent = getTrueOffsetParent$1(offsetParent, polyfill);
+        }
+        if (offsetParent && (getNodeName$1(offsetParent) === "html" || getNodeName$1(offsetParent) === "body" && getComputedStyle$2(offsetParent).position === "static" && !isContainingBlock(offsetParent))) {
+            return window2;
+        }
+        return offsetParent || getContainingBlock$1(element2) || window2;
+    }
+    const getElementRects = async function(data2) {
+        const getOffsetParentFn = this.getOffsetParent || getOffsetParent$1;
+        const getDimensionsFn = this.getDimensions;
+        const floatingDimensions = await getDimensionsFn(data2.floating);
+        return {
+            reference: getRectRelativeToOffsetParent(data2.reference, await getOffsetParentFn(data2.floating), data2.strategy),
+            floating: {
+                x: 0,
+                y: 0,
+                width: floatingDimensions.width,
+                height: floatingDimensions.height
+            }
+        };
+    };
+
+    function isRTL(element2) {
+        return getComputedStyle$2(element2).direction === "rtl";
+    }
+    const platform = {
+        convertOffsetParentRelativeRectToViewportRelativeRect,
+        getDocumentElement: getDocumentElement$1,
+        getClippingRect: getClippingRect$1,
+        getOffsetParent: getOffsetParent$1,
+        getElementRects,
+        getClientRects,
+        getDimensions,
+        getScale: getScale$1,
+        isElement: isElement$4,
+        isRTL
+    };
+
+    function observeMove(element2, onMove) {
+        let io2 = null;
+        let timeoutId;
+        const root2 = getDocumentElement$1(element2);
+
+        function cleanup() {
+            var _io;
+            clearTimeout(timeoutId);
+            (_io = io2) == null || _io.disconnect();
+            io2 = null;
+        }
+
+        function refresh(skip, threshold) {
+            if (skip === void 0) {
+                skip = false;
+            }
+            if (threshold === void 0) {
+                threshold = 1;
+            }
+            cleanup();
+            const {
+                left: left2,
+                top: top2,
+                width,
+                height
+            } = element2.getBoundingClientRect();
+            if (!skip) {
+                onMove();
+            }
+            if (!width || !height) {
+                return;
+            }
+            const insetTop = floor(top2);
+            const insetRight = floor(root2.clientWidth - (left2 + width));
+            const insetBottom = floor(root2.clientHeight - (top2 + height));
+            const insetLeft = floor(left2);
+            const rootMargin = -insetTop + "px " + -insetRight + "px " + -insetBottom + "px " + -insetLeft + "px";
+            const options = {
+                rootMargin,
+                threshold: max$4(0, min$3(1, threshold)) || 1
+            };
+            let isFirstUpdate = true;
+
+            function handleObserve(entries) {
+                const ratio = entries[0].intersectionRatio;
+                if (ratio !== threshold) {
+                    if (!isFirstUpdate) {
+                        return refresh();
+                    }
+                    if (!ratio) {
+                        timeoutId = setTimeout(() => {
+                            refresh(false, 1e-7);
+                        }, 1e3);
+                    } else {
+                        refresh(false, ratio);
+                    }
+                }
+                isFirstUpdate = false;
+            }
+            try {
+                io2 = new IntersectionObserver(handleObserve, {
+                    ...options,
+                    root: root2.ownerDocument
+                });
+            } catch (e3) {
+                io2 = new IntersectionObserver(handleObserve, options);
+            }
+            io2.observe(element2);
+        }
+        refresh(true);
+        return cleanup;
+    }
+
+    function autoUpdate(reference2, floating, update2, options) {
+        if (options === void 0) {
+            options = {};
+        }
+        const {
+            ancestorScroll = true,
+                ancestorResize = true,
+                elementResize = typeof ResizeObserver === "function",
+                layoutShift = typeof IntersectionObserver === "function",
+                animationFrame = false
+        } = options;
+        const referenceEl = unwrapElement(reference2);
+        const ancestors = ancestorScroll || ancestorResize ? [...referenceEl ? getOverflowAncestors(referenceEl) : [], ...getOverflowAncestors(floating)] : [];
+        ancestors.forEach((ancestor) => {
+            ancestorScroll && ancestor.addEventListener("scroll", update2, {
+                passive: true
+            });
+            ancestorResize && ancestor.addEventListener("resize", update2);
+        });
+        const cleanupIo = referenceEl && layoutShift ? observeMove(referenceEl, update2) : null;
+        let reobserveFrame = -1;
+        let resizeObserver = null;
+        if (elementResize) {
+            resizeObserver = new ResizeObserver((_ref2) => {
+                let [firstEntry] = _ref2;
+                if (firstEntry && firstEntry.target === referenceEl && resizeObserver) {
+                    resizeObserver.unobserve(floating);
+                    cancelAnimationFrame(reobserveFrame);
+                    reobserveFrame = requestAnimationFrame(() => {
+                        var _resizeObserver;
+                        (_resizeObserver = resizeObserver) == null || _resizeObserver.observe(floating);
+                    });
+                }
+                update2();
+            });
+            if (referenceEl && !animationFrame) {
+                resizeObserver.observe(referenceEl);
+            }
+            resizeObserver.observe(floating);
+        }
+        let frameId;
+        let prevRefRect = animationFrame ? getBoundingClientRect$1(reference2) : null;
+        if (animationFrame) {
+            frameLoop();
+        }
+
+        function frameLoop() {
+            const nextRefRect = getBoundingClientRect$1(reference2);
+            if (prevRefRect && (nextRefRect.x !== prevRefRect.x || nextRefRect.y !== prevRefRect.y || nextRefRect.width !== prevRefRect.width || nextRefRect.height !== prevRefRect.height)) {
+                update2();
+            }
+            prevRefRect = nextRefRect;
+            frameId = requestAnimationFrame(frameLoop);
+        }
+        update2();
+        return () => {
+            var _resizeObserver2;
+            ancestors.forEach((ancestor) => {
+                ancestorScroll && ancestor.removeEventListener("scroll", update2);
+                ancestorResize && ancestor.removeEventListener("resize", update2);
+            });
+            cleanupIo == null || cleanupIo();
+            (_resizeObserver2 = resizeObserver) == null || _resizeObserver2.disconnect();
+            resizeObserver = null;
+            if (animationFrame) {
+                cancelAnimationFrame(frameId);
+            }
+        };
+    }
+    const offset$2 = offset$3;
+    autoPlacement;
+    const shift$1 = shift$2;
+    const flip$2 = flip$3;
+    const size$1 = size$2;
+    hide$2;
+    arrow$2;
+    inline;
+    limitShift;
+    const computePosition = (reference2, floating, options) => {
+        const cache2 = /* @__PURE__ */ new Map();
+        const mergedOptions = {
+            platform,
+            ...options
+        };
+        const platformWithCache = {
+            ...mergedOptions.platform,
+            _c: cache2
+        };
+        return computePosition$1(reference2, floating, {
+            ...mergedOptions,
+            platform: platformWithCache
+        });
+    };
+    var index$4 = typeof document !== "undefined" ? React.useLayoutEffect : React.useEffect;
+
+    function deepEqual(a2, b2) {
+        if (a2 === b2) {
+            return true;
+        }
+        if (typeof a2 !== typeof b2) {
+            return false;
+        }
+        if (typeof a2 === "function" && a2.toString() === b2.toString()) {
+            return true;
+        }
+        let length;
+        let i2;
+        let keys2;
+        if (a2 && b2 && typeof a2 === "object") {
+            if (Array.isArray(a2)) {
+                length = a2.length;
+                if (length !== b2.length)
+                    return false;
+                for (i2 = length; i2-- !== 0;) {
+                    if (!deepEqual(a2[i2], b2[i2])) {
+                        return false;
+                    }
+                }
+                return true;
+            }
+            keys2 = Object.keys(a2);
+            length = keys2.length;
+            if (length !== Object.keys(b2).length) {
+                return false;
+            }
+            for (i2 = length; i2-- !== 0;) {
+                if (!{}.hasOwnProperty.call(b2, keys2[i2])) {
+                    return false;
+                }
+            }
+            for (i2 = length; i2-- !== 0;) {
+                const key = keys2[i2];
+                if (key === "_owner" && a2.$$typeof) {
+                    continue;
+                }
+                if (!deepEqual(a2[key], b2[key])) {
+                    return false;
+                }
+            }
+            return true;
+        }
+        return a2 !== a2 && b2 !== b2;
+    }
+
+    function getDPR(element2) {
+        if (typeof window === "undefined") {
+            return 1;
+        }
+        const win = element2.ownerDocument.defaultView || window;
+        return win.devicePixelRatio || 1;
+    }
+
+    function roundByDPR(element2, value) {
+        const dpr = getDPR(element2);
+        return Math.round(value * dpr) / dpr;
+    }
+
+    function useLatestRef$1(value) {
+        const ref2 = React__namespace.useRef(value);
+        index$4(() => {
+            ref2.current = value;
+        });
+        return ref2;
+    }
+
+    function useFloating$1(options) {
+        if (options === void 0) {
+            options = {};
+        }
+        const {
+            placement = "bottom",
+                strategy = "absolute",
+                middleware = [],
+                platform: platform2,
+                elements: {
+                    reference: externalReference,
+                    floating: externalFloating
+                } = {},
+                transform = true,
+                whileElementsMounted,
+                open
+        } = options;
+        const [data2, setData] = React__namespace.useState({
+            x: 0,
+            y: 0,
+            strategy,
+            placement,
+            middlewareData: {},
+            isPositioned: false
+        });
+        const [latestMiddleware, setLatestMiddleware] = React__namespace.useState(middleware);
+        if (!deepEqual(latestMiddleware, middleware)) {
+            setLatestMiddleware(middleware);
+        }
+        const [_reference, _setReference] = React__namespace.useState(null);
+        const [_floating, _setFloating] = React__namespace.useState(null);
+        const setReference = React__namespace.useCallback((node2) => {
+            if (node2 !== referenceRef.current) {
+                referenceRef.current = node2;
+                _setReference(node2);
+            }
+        }, []);
+        const setFloating = React__namespace.useCallback((node2) => {
+            if (node2 !== floatingRef.current) {
+                floatingRef.current = node2;
+                _setFloating(node2);
+            }
+        }, []);
+        const referenceEl = externalReference || _reference;
+        const floatingEl = externalFloating || _floating;
+        const referenceRef = React__namespace.useRef(null);
+        const floatingRef = React__namespace.useRef(null);
+        const dataRef = React__namespace.useRef(data2);
+        const hasWhileElementsMounted = whileElementsMounted != null;
+        const whileElementsMountedRef = useLatestRef$1(whileElementsMounted);
+        const platformRef = useLatestRef$1(platform2);
+        const update2 = React__namespace.useCallback(() => {
+            if (!referenceRef.current || !floatingRef.current) {
+                return;
+            }
+            const config2 = {
+                placement,
+                strategy,
+                middleware: latestMiddleware
+            };
+            if (platformRef.current) {
+                config2.platform = platformRef.current;
+            }
+            computePosition(referenceRef.current, floatingRef.current, config2).then((data3) => {
+                const fullData = {
+                    ...data3,
+                    isPositioned: true
+                };
+                if (isMountedRef.current && !deepEqual(dataRef.current, fullData)) {
+                    dataRef.current = fullData;
+                    ReactDOM__namespace.flushSync(() => {
+                        setData(fullData);
+                    });
+                }
+            });
+        }, [latestMiddleware, placement, strategy, platformRef]);
+        index$4(() => {
+            if (open === false && dataRef.current.isPositioned) {
+                dataRef.current.isPositioned = false;
+                setData((data3) => ({
+                    ...data3,
+                    isPositioned: false
+                }));
+            }
+        }, [open]);
+        const isMountedRef = React__namespace.useRef(false);
+        index$4(() => {
+            isMountedRef.current = true;
+            return () => {
+                isMountedRef.current = false;
+            };
+        }, []);
+        index$4(() => {
+            if (referenceEl)
+                referenceRef.current = referenceEl;
+            if (floatingEl)
+                floatingRef.current = floatingEl;
+            if (referenceEl && floatingEl) {
+                if (whileElementsMountedRef.current) {
+                    return whileElementsMountedRef.current(referenceEl, floatingEl, update2);
+                }
+                update2();
+            }
+        }, [referenceEl, floatingEl, update2, whileElementsMountedRef, hasWhileElementsMounted]);
+        const refs = React__namespace.useMemo(() => ({
+            reference: referenceRef,
+            floating: floatingRef,
+            setReference,
+            setFloating
+        }), [setReference, setFloating]);
+        const elements = React__namespace.useMemo(() => ({
+            reference: referenceEl,
+            floating: floatingEl
+        }), [referenceEl, floatingEl]);
+        const floatingStyles = React__namespace.useMemo(() => {
+            const initialStyles = {
+                position: strategy,
+                left: 0,
+                top: 0
+            };
+            if (!elements.floating) {
+                return initialStyles;
+            }
+            const x2 = roundByDPR(elements.floating, data2.x);
+            const y2 = roundByDPR(elements.floating, data2.y);
+            if (transform) {
+                return {
+                    ...initialStyles,
+                    transform: "translate(" + x2 + "px, " + y2 + "px)",
+                    ...getDPR(elements.floating) >= 1.5 && {
+                        willChange: "transform"
+                    }
+                };
+            }
+            return {
+                position: strategy,
+                left: x2,
+                top: y2
+            };
+        }, [strategy, transform, elements.floating, data2.x, data2.y]);
+        return React__namespace.useMemo(() => ({
+            ...data2,
+            update: update2,
+            refs,
+            elements,
+            floatingStyles
+        }), [data2, update2, refs, elements, floatingStyles]);
+    }
+    const SafeReact = {
+        ...React__namespace
+    };
+    const useInsertionEffect = SafeReact.useInsertionEffect;
+    const useSafeInsertionEffect = useInsertionEffect || ((fn2) => fn2());
+
+    function useEffectEvent(callback) {
+        const ref2 = React__namespace.useRef(() => {});
+        useSafeInsertionEffect(() => {
+            ref2.current = callback;
+        });
+        return React__namespace.useCallback(function() {
+            for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {
+                args[_key] = arguments[_key];
+            }
+            return ref2.current == null ? void 0 : ref2.current(...args);
+        }, []);
+    }
+    var index$3 = typeof document !== "undefined" ? React.useLayoutEffect : React.useEffect;
+    let serverHandoffComplete = false;
+    let count$1 = 0;
+    const genId = () => "floating-ui-" + Math.random().toString(36).slice(2, 6) + count$1++;
+
+    function useFloatingId() {
+        const [id2, setId] = React__namespace.useState(() => serverHandoffComplete ? genId() : void 0);
+        index$3(() => {
+            if (id2 == null) {
+                setId(genId());
+            }
+        }, []);
+        React__namespace.useEffect(() => {
+            serverHandoffComplete = true;
+        }, []);
+        return id2;
+    }
+    const useReactId = SafeReact.useId;
+    const useId = useReactId || useFloatingId;
+
+    function createPubSub() {
+        const map2 = /* @__PURE__ */ new Map();
+        return {
+            emit(event2, data2) {
+                var _map$get;
+                (_map$get = map2.get(event2)) == null || _map$get.forEach((handler) => handler(data2));
+            },
+            on(event2, listener2) {
+                map2.set(event2, [...map2.get(event2) || [], listener2]);
+            },
+            off(event2, listener2) {
+                var _map$get2;
+                map2.set(event2, ((_map$get2 = map2.get(event2)) == null ? void 0 : _map$get2.filter((l2) => l2 !== listener2)) || []);
+            }
+        };
+    }
+    const FloatingNodeContext = /* @__PURE__ */ React__namespace.createContext(null);
+    const FloatingTreeContext = /* @__PURE__ */ React__namespace.createContext(null);
+    const useFloatingParentNodeId = () => {
+        var _React$useContext;
+        return ((_React$useContext = React__namespace.useContext(FloatingNodeContext)) == null ? void 0 : _React$useContext.id) || null;
+    };
+    const useFloatingTree = () => React__namespace.useContext(FloatingTreeContext);
+
+    function createAttribute(name2) {
+        return "data-floating-ui-" + name2;
+    }
+
+    function getChildren$3(nodes, id2) {
+        let allChildren = nodes.filter((node2) => {
+            var _node$context;
+            return node2.parentId === id2 && ((_node$context = node2.context) == null ? void 0 : _node$context.open);
+        });
+        let currentChildren = allChildren;
+        while (currentChildren.length) {
+            currentChildren = nodes.filter((node2) => {
+                var _currentChildren;
+                return (_currentChildren = currentChildren) == null ? void 0 : _currentChildren.some((n2) => {
+                    var _node$context2;
+                    return node2.parentId === n2.id && ((_node$context2 = node2.context) == null ? void 0 : _node$context2.open);
+                });
+            });
+            allChildren = allChildren.concat(currentChildren);
+        }
+        return allChildren;
+    }
+
+    function isButtonTarget(event2) {
+        return isHTMLElement$1(event2.target) && event2.target.tagName === "BUTTON";
+    }
+
+    function isSpaceIgnored(element2) {
+        return isTypeableElement(element2);
+    }
+
+    function useClick(context2, props) {
+        if (props === void 0) {
+            props = {};
+        }
+        const {
+            open,
+            onOpenChange,
+            dataRef,
+            elements: {
+                domReference
+            }
+        } = context2;
+        const {
+            enabled = true,
+                event: eventOption = "click",
+                toggle = true,
+                ignoreMouse = false,
+                keyboardHandlers = true
+        } = props;
+        const pointerTypeRef = React__namespace.useRef();
+        const didKeyDownRef = React__namespace.useRef(false);
+        return React__namespace.useMemo(() => {
+            if (!enabled)
+                return {};
+            return {
+                reference: {
+                    onPointerDown(event2) {
+                        pointerTypeRef.current = event2.pointerType;
+                    },
+                    onMouseDown(event2) {
+                        if (event2.button !== 0) {
+                            return;
+                        }
+                        if (isMouseLikePointerType(pointerTypeRef.current, true) && ignoreMouse) {
+                            return;
+                        }
+                        if (eventOption === "click") {
+                            return;
+                        }
+                        if (open && toggle && (dataRef.current.openEvent ? dataRef.current.openEvent.type === "mousedown" : true)) {
+                            onOpenChange(false, event2.nativeEvent, "click");
+                        } else {
+                            event2.preventDefault();
+                            onOpenChange(true, event2.nativeEvent, "click");
+                        }
+                    },
+                    onClick(event2) {
+                        if (eventOption === "mousedown" && pointerTypeRef.current) {
+                            pointerTypeRef.current = void 0;
+                            return;
+                        }
+                        if (isMouseLikePointerType(pointerTypeRef.current, true) && ignoreMouse) {
+                            return;
+                        }
+                        if (open && toggle && (dataRef.current.openEvent ? dataRef.current.openEvent.type === "click" : true)) {
+                            onOpenChange(false, event2.nativeEvent, "click");
+                        } else {
+                            onOpenChange(true, event2.nativeEvent, "click");
+                        }
+                    },
+                    onKeyDown(event2) {
+                        pointerTypeRef.current = void 0;
+                        if (event2.defaultPrevented || !keyboardHandlers || isButtonTarget(event2)) {
+                            return;
+                        }
+                        if (event2.key === " " && !isSpaceIgnored(domReference)) {
+                            event2.preventDefault();
+                            didKeyDownRef.current = true;
+                        }
+                        if (event2.key === "Enter") {
+                            if (open && toggle) {
+                                onOpenChange(false, event2.nativeEvent, "click");
+                            } else {
+                                onOpenChange(true, event2.nativeEvent, "click");
+                            }
+                        }
+                    },
+                    onKeyUp(event2) {
+                        if (event2.defaultPrevented || !keyboardHandlers || isButtonTarget(event2) || isSpaceIgnored(domReference)) {
+                            return;
+                        }
+                        if (event2.key === " " && didKeyDownRef.current) {
+                            didKeyDownRef.current = false;
+                            if (open && toggle) {
+                                onOpenChange(false, event2.nativeEvent, "click");
+                            } else {
+                                onOpenChange(true, event2.nativeEvent, "click");
+                            }
+                        }
+                    }
+                }
+            };
+        }, [enabled, dataRef, eventOption, ignoreMouse, keyboardHandlers, domReference, toggle, open, onOpenChange]);
+    }
+    const bubbleHandlerKeys = {
+        pointerdown: "onPointerDown",
+        mousedown: "onMouseDown",
+        click: "onClick"
+    };
+    const captureHandlerKeys = {
+        pointerdown: "onPointerDownCapture",
+        mousedown: "onMouseDownCapture",
+        click: "onClickCapture"
+    };
+    const normalizeProp = (normalizable) => {
+        var _normalizable$escapeK, _normalizable$outside;
+        return {
+            escapeKey: typeof normalizable === "boolean" ? normalizable : (_normalizable$escapeK = normalizable == null ? void 0 : normalizable.escapeKey) != null ? _normalizable$escapeK : false,
+            outsidePress: typeof normalizable === "boolean" ? normalizable : (_normalizable$outside = normalizable == null ? void 0 : normalizable.outsidePress) != null ? _normalizable$outside : true
+        };
+    };
+
+    function useDismiss(context2, props) {
+        if (props === void 0) {
+            props = {};
+        }
+        const {
+            open,
+            onOpenChange,
+            nodeId,
+            elements: {
+                reference: reference2,
+                domReference,
+                floating
+            },
+            dataRef
+        } = context2;
+        const {
+            enabled = true,
+                escapeKey = true,
+                outsidePress: unstable_outsidePress = true,
+                outsidePressEvent = "pointerdown",
+                referencePress = false,
+                referencePressEvent = "pointerdown",
+                ancestorScroll = false,
+                bubbles,
+                capture
+        } = props;
+        const tree = useFloatingTree();
+        const outsidePressFn = useEffectEvent(typeof unstable_outsidePress === "function" ? unstable_outsidePress : () => false);
+        const outsidePress = typeof unstable_outsidePress === "function" ? outsidePressFn : unstable_outsidePress;
+        const insideReactTreeRef = React__namespace.useRef(false);
+        const endedOrStartedInsideRef = React__namespace.useRef(false);
+        const {
+            escapeKey: escapeKeyBubbles,
+            outsidePress: outsidePressBubbles
+        } = normalizeProp(bubbles);
+        const {
+            escapeKey: escapeKeyCapture,
+            outsidePress: outsidePressCapture
+        } = normalizeProp(capture);
+        const closeOnEscapeKeyDown = useEffectEvent((event2) => {
+            if (!open || !enabled || !escapeKey || event2.key !== "Escape") {
+                return;
+            }
+            const children2 = tree ? getChildren$3(tree.nodesRef.current, nodeId) : [];
+            if (!escapeKeyBubbles) {
+                event2.stopPropagation();
+                if (children2.length > 0) {
+                    let shouldDismiss = true;
+                    children2.forEach((child) => {
+                        var _child$context;
+                        if ((_child$context = child.context) != null && _child$context.open && !child.context.dataRef.current.__escapeKeyBubbles) {
+                            shouldDismiss = false;
+                            return;
+                        }
+                    });
+                    if (!shouldDismiss) {
+                        return;
+                    }
+                }
+            }
+            onOpenChange(false, isReactEvent(event2) ? event2.nativeEvent : event2, "escape-key");
+        });
+        const closeOnEscapeKeyDownCapture = useEffectEvent((event2) => {
+            var _getTarget2;
+            const callback = () => {
+                var _getTarget;
+                closeOnEscapeKeyDown(event2);
+                (_getTarget = getTarget(event2)) == null || _getTarget.removeEventListener("keydown", callback);
+            };
+            (_getTarget2 = getTarget(event2)) == null || _getTarget2.addEventListener("keydown", callback);
+        });
+        const closeOnPressOutside = useEffectEvent((event2) => {
+            const insideReactTree = insideReactTreeRef.current;
+            insideReactTreeRef.current = false;
+            const endedOrStartedInside = endedOrStartedInsideRef.current;
+            endedOrStartedInsideRef.current = false;
+            if (outsidePressEvent === "click" && endedOrStartedInside) {
+                return;
+            }
+            if (insideReactTree) {
+                return;
+            }
+            if (typeof outsidePress === "function" && !outsidePress(event2)) {
+                return;
+            }
+            const target = getTarget(event2);
+            const inertSelector = "[" + createAttribute("inert") + "]";
+            const markers = getDocument(floating).querySelectorAll(inertSelector);
+            let targetRootAncestor = isElement$4(target) ? target : null;
+            while (targetRootAncestor && !isLastTraversableNode(targetRootAncestor)) {
+                const nextParent = getParentNode$1(targetRootAncestor);
+                if (isLastTraversableNode(nextParent) || !isElement$4(nextParent)) {
+                    break;
+                }
+                targetRootAncestor = nextParent;
+            }
+            if (markers.length && isElement$4(target) && !isRootElement(target) && !contains$2(target, floating) && Array.from(markers).every((marker) => !contains$2(targetRootAncestor, marker))) {
+                return;
+            }
+            if (isHTMLElement$1(target) && floating) {
+                const canScrollX = target.clientWidth > 0 && target.scrollWidth > target.clientWidth;
+                const canScrollY = target.clientHeight > 0 && target.scrollHeight > target.clientHeight;
+                let xCond = canScrollY && event2.offsetX > target.clientWidth;
+                if (canScrollY) {
+                    const isRTL2 = getComputedStyle$2(target).direction === "rtl";
+                    if (isRTL2) {
+                        xCond = event2.offsetX <= target.offsetWidth - target.clientWidth;
+                    }
+                }
+                if (xCond || canScrollX && event2.offsetY > target.clientHeight) {
+                    return;
+                }
+            }
+            const targetIsInsideChildren = tree && getChildren$3(tree.nodesRef.current, nodeId).some((node2) => {
+                var _node$context;
+                return isEventTargetWithin(event2, (_node$context = node2.context) == null ? void 0 : _node$context.elements.floating);
+            });
+            if (isEventTargetWithin(event2, floating) || isEventTargetWithin(event2, domReference) || targetIsInsideChildren) {
+                return;
+            }
+            const children2 = tree ? getChildren$3(tree.nodesRef.current, nodeId) : [];
+            if (children2.length > 0) {
+                let shouldDismiss = true;
+                children2.forEach((child) => {
+                    var _child$context2;
+                    if ((_child$context2 = child.context) != null && _child$context2.open && !child.context.dataRef.current.__outsidePressBubbles) {
+                        shouldDismiss = false;
+                        return;
+                    }
+                });
+                if (!shouldDismiss) {
+                    return;
+                }
+            }
+            onOpenChange(false, event2, "outside-press");
+        });
+        const closeOnPressOutsideCapture = useEffectEvent((event2) => {
+            var _getTarget4;
+            const callback = () => {
+                var _getTarget3;
+                closeOnPressOutside(event2);
+                (_getTarget3 = getTarget(event2)) == null || _getTarget3.removeEventListener(outsidePressEvent, callback);
+            };
+            (_getTarget4 = getTarget(event2)) == null || _getTarget4.addEventListener(outsidePressEvent, callback);
+        });
+        React__namespace.useEffect(() => {
+            if (!open || !enabled) {
+                return;
+            }
+            dataRef.current.__escapeKeyBubbles = escapeKeyBubbles;
+            dataRef.current.__outsidePressBubbles = outsidePressBubbles;
+
+            function onScroll(event2) {
+                onOpenChange(false, event2, "ancestor-scroll");
+            }
+            const doc2 = getDocument(floating);
+            escapeKey && doc2.addEventListener("keydown", escapeKeyCapture ? closeOnEscapeKeyDownCapture : closeOnEscapeKeyDown, escapeKeyCapture);
+            outsidePress && doc2.addEventListener(outsidePressEvent, outsidePressCapture ? closeOnPressOutsideCapture : closeOnPressOutside, outsidePressCapture);
+            let ancestors = [];
+            if (ancestorScroll) {
+                if (isElement$4(domReference)) {
+                    ancestors = getOverflowAncestors(domReference);
+                }
+                if (isElement$4(floating)) {
+                    ancestors = ancestors.concat(getOverflowAncestors(floating));
+                }
+                if (!isElement$4(reference2) && reference2 && reference2.contextElement) {
+                    ancestors = ancestors.concat(getOverflowAncestors(reference2.contextElement));
+                }
+            }
+            ancestors = ancestors.filter((ancestor) => {
+                var _doc$defaultView;
+                return ancestor !== ((_doc$defaultView = doc2.defaultView) == null ? void 0 : _doc$defaultView.visualViewport);
+            });
+            ancestors.forEach((ancestor) => {
+                ancestor.addEventListener("scroll", onScroll, {
+                    passive: true
+                });
+            });
+            return () => {
+                escapeKey && doc2.removeEventListener("keydown", escapeKeyCapture ? closeOnEscapeKeyDownCapture : closeOnEscapeKeyDown, escapeKeyCapture);
+                outsidePress && doc2.removeEventListener(outsidePressEvent, outsidePressCapture ? closeOnPressOutsideCapture : closeOnPressOutside, outsidePressCapture);
+                ancestors.forEach((ancestor) => {
+                    ancestor.removeEventListener("scroll", onScroll);
+                });
+            };
+        }, [dataRef, floating, domReference, reference2, escapeKey, outsidePress, outsidePressEvent, open, onOpenChange, ancestorScroll, enabled, escapeKeyBubbles, outsidePressBubbles, closeOnEscapeKeyDown, escapeKeyCapture, closeOnEscapeKeyDownCapture, closeOnPressOutside, outsidePressCapture, closeOnPressOutsideCapture]);
+        React__namespace.useEffect(() => {
+            insideReactTreeRef.current = false;
+        }, [outsidePress, outsidePressEvent]);
+        return React__namespace.useMemo(() => {
+            if (!enabled) {
+                return {};
+            }
+            return {
+                reference: {
+                    onKeyDown: closeOnEscapeKeyDown,
+                    [bubbleHandlerKeys[referencePressEvent]]: (event2) => {
+                        if (referencePress) {
+                            onOpenChange(false, event2.nativeEvent, "reference-press");
+                        }
+                    }
+                },
+                floating: {
+                    onKeyDown: closeOnEscapeKeyDown,
+                    onMouseDown() {
+                        endedOrStartedInsideRef.current = true;
+                    },
+                    onMouseUp() {
+                        endedOrStartedInsideRef.current = true;
+                    },
+                    [captureHandlerKeys[outsidePressEvent]]: () => {
+                        insideReactTreeRef.current = true;
+                    }
+                }
+            };
+        }, [enabled, referencePress, outsidePressEvent, referencePressEvent, onOpenChange, closeOnEscapeKeyDown]);
+    }
+
+    function useFloating(options) {
+        var _options$elements;
+        if (options === void 0) {
+            options = {};
+        }
+        const {
+            open = false,
+                onOpenChange: unstable_onOpenChange,
+                nodeId
+        } = options;
+        const [_domReference, setDomReference] = React__namespace.useState(null);
+        const [positionReference, _setPositionReference] = React__namespace.useState(null);
+        const optionDomReference = (_options$elements = options.elements) == null ? void 0 : _options$elements.reference;
+        const domReference = optionDomReference || _domReference;
+        index$3(() => {
+            if (domReference) {
+                domReferenceRef.current = domReference;
+            }
+        }, [domReference]);
+        const position2 = useFloating$1({
+            ...options,
+            elements: {
+                ...options.elements,
+                ...positionReference && {
+                    reference: positionReference
+                }
+            }
+        });
+        const tree = useFloatingTree();
+        const nested = useFloatingParentNodeId() != null;
+        const onOpenChange = useEffectEvent((open2, event2, reason) => {
+            dataRef.current.openEvent = open2 ? event2 : void 0;
+            events2.emit("openchange", {
+                open: open2,
+                event: event2,
+                reason,
+                nested
+            });
+            unstable_onOpenChange == null || unstable_onOpenChange(open2, event2, reason);
+        });
+        const domReferenceRef = React__namespace.useRef(null);
+        const dataRef = React__namespace.useRef({});
+        const events2 = React__namespace.useState(() => createPubSub())[0];
+        const floatingId = useId();
+        const setPositionReference = React__namespace.useCallback((node2) => {
+            const computedPositionReference = isElement$4(node2) ? {
+                getBoundingClientRect: () => node2.getBoundingClientRect(),
+                contextElement: node2
+            } : node2;
+            _setPositionReference(computedPositionReference);
+            position2.refs.setReference(computedPositionReference);
+        }, [position2.refs]);
+        const setReference = React__namespace.useCallback((node2) => {
+            if (isElement$4(node2) || node2 === null) {
+                domReferenceRef.current = node2;
+                setDomReference(node2);
+            }
+            if (isElement$4(position2.refs.reference.current) || position2.refs.reference.current === null || node2 !== null && !isElement$4(node2)) {
+                position2.refs.setReference(node2);
+            }
+        }, [position2.refs]);
+        const refs = React__namespace.useMemo(() => ({
+            ...position2.refs,
+            setReference,
+            setPositionReference,
+            domReference: domReferenceRef
+        }), [position2.refs, setReference, setPositionReference]);
+        const elements = React__namespace.useMemo(() => ({
+            ...position2.elements,
+            domReference
+        }), [position2.elements, domReference]);
+        const context2 = React__namespace.useMemo(() => ({
+            ...position2,
+            refs,
+            elements,
+            dataRef,
+            nodeId,
+            floatingId,
+            events: events2,
+            open,
+            onOpenChange
+        }), [position2, nodeId, floatingId, events2, open, onOpenChange, refs, elements]);
+        index$3(() => {
+            const node2 = tree == null ? void 0 : tree.nodesRef.current.find((node3) => node3.id === nodeId);
+            if (node2) {
+                node2.context = context2;
+            }
+        });
+        return React__namespace.useMemo(() => ({
+            ...position2,
+            context: context2,
+            refs,
+            elements
+        }), [position2, refs, elements, context2]);
+    }
+    const ACTIVE_KEY = "active";
+    const SELECTED_KEY = "selected";
+
+    function mergeProps(userProps, propsList, elementKey) {
+        const map2 = /* @__PURE__ */ new Map();
+        const isItem2 = elementKey === "item";
+        let domUserProps = userProps;
+        if (isItem2 && userProps) {
+            const {
+                [ACTIVE_KEY]: _2,
+                [SELECTED_KEY]: __,
+                ...validProps
+            } = userProps;
+            domUserProps = validProps;
+        }
+        return {
+            ...elementKey === "floating" && {
+                tabIndex: -1
+            },
+            ...domUserProps,
+            ...propsList.map((value) => {
+                const propsOrGetProps = value ? value[elementKey] : null;
+                if (typeof propsOrGetProps === "function") {
+                    return userProps ? propsOrGetProps(userProps) : null;
+                }
+                return propsOrGetProps;
+            }).concat(userProps).reduce((acc, props) => {
+                if (!props) {
+                    return acc;
+                }
+                Object.entries(props).forEach((_ref2) => {
+                    let [key, value] = _ref2;
+                    if (isItem2 && [ACTIVE_KEY, SELECTED_KEY].includes(key)) {
+                        return;
+                    }
+                    if (key.indexOf("on") === 0) {
+                        if (!map2.has(key)) {
+                            map2.set(key, []);
+                        }
+                        if (typeof value === "function") {
+                            var _map$get;
+                            (_map$get = map2.get(key)) == null || _map$get.push(value);
+                            acc[key] = function() {
+                                var _map$get2;
+                                for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {
+                                    args[_key] = arguments[_key];
+                                }
+                                return (_map$get2 = map2.get(key)) == null ? void 0 : _map$get2.map((fn2) => fn2(...args)).find((val) => val !== void 0);
+                            };
+                        }
+                    } else {
+                        acc[key] = value;
+                    }
+                });
+                return acc;
+            }, {})
+        };
+    }
+
+    function useInteractions(propsList) {
+        if (propsList === void 0) {
+            propsList = [];
+        }
+        const deps = propsList;
+        const getReferenceProps = React__namespace.useCallback(
+            (userProps) => mergeProps(userProps, propsList, "reference"),
+            deps
+        );
+        const getFloatingProps = React__namespace.useCallback(
+            (userProps) => mergeProps(userProps, propsList, "floating"),
+            deps
+        );
+        const getItemProps = React__namespace.useCallback(
+            (userProps) => mergeProps(userProps, propsList, "item"),
+            propsList.map((key) => key == null ? void 0 : key.item)
+        );
+        return React__namespace.useMemo(() => ({
+            getReferenceProps,
+            getFloatingProps,
+            getItemProps
+        }), [getReferenceProps, getFloatingProps, getItemProps]);
+    }
+    const componentRoleToAriaRoleMap = /* @__PURE__ */ new Map([
+        ["select", "listbox"],
+        ["combobox", "listbox"],
+        ["label", false]
+    ]);
+
+    function useRole(context2, props) {
+        var _componentRoleToAriaR;
+        if (props === void 0) {
+            props = {};
+        }
+        const {
+            open,
+            floatingId
+        } = context2;
+        const {
+            enabled = true,
+                role = "dialog"
+        } = props;
+        const ariaRole = (_componentRoleToAriaR = componentRoleToAriaRoleMap.get(role)) != null ? _componentRoleToAriaR : role;
+        const referenceId = useId();
+        const parentId = useFloatingParentNodeId();
+        const isNested = parentId != null;
+        return React__namespace.useMemo(() => {
+            if (!enabled)
+                return {};
+            const floatingProps = {
+                id: floatingId,
+                ...ariaRole && {
+                    role: ariaRole
+                }
+            };
+            if (ariaRole === "tooltip" || role === "label") {
+                return {
+                    reference: {
+                        ["aria-" + (role === "label" ? "labelledby" : "describedby")]: open ? floatingId : void 0
+                    },
+                    floating: floatingProps
+                };
+            }
+            return {
+                reference: {
+                    "aria-expanded": open ? "true" : "false",
+                    "aria-haspopup": ariaRole === "alertdialog" ? "dialog" : ariaRole,
+                    "aria-controls": open ? floatingId : void 0,
+                    ...ariaRole === "listbox" && {
+                        role: "combobox"
+                    },
+                    ...ariaRole === "menu" && {
+                        id: referenceId
+                    },
+                    ...ariaRole === "menu" && isNested && {
+                        role: "menuitem"
+                    },
+                    ...role === "select" && {
+                        "aria-autocomplete": "none"
+                    },
+                    ...role === "combobox" && {
+                        "aria-autocomplete": "list"
+                    }
+                },
+                floating: {
+                    ...floatingProps,
+                    ...ariaRole === "menu" && {
+                        "aria-labelledby": referenceId
+                    }
+                },
+                item(_ref2) {
+                    let {
+                        active,
+                        selected
+                    } = _ref2;
+                    const commonProps = {
+                        role: "option",
+                        ...active && {
+                            id: floatingId + "-option"
+                        }
+                    };
+                    switch (role) {
+                        case "select":
+                            return {
+                                ...commonProps,
+                                "aria-selected": active && selected
+                            };
+                        case "combobox": {
+                            return {
+                                ...commonProps,
+                                ...active && {
+                                    "aria-selected": true
+                                }
+                            };
+                        }
+                    }
+                    return {};
+                }
+            };
+        }, [enabled, role, ariaRole, open, floatingId, referenceId, isNested]);
+    }
+    const matchWidthToReference = (delta = 0) => size$1({
+        apply({
+            rects,
+            elements
+        }) {
+            Object.assign(elements.floating.style, {
+                width: `${rects.reference.width + delta}px`
+            });
+        }
+    });
     const AccordionItemWrapper = styled__default.default.div`
     width: 100%;
     background-color: ${(props) => {
     var _a3;
     return (_a3 = props.backgroundColor) !== null && _a3 !== void 0 ? _a3 : props.theme.colors.blue1;
   }};
     border: 1px solid ${(props) => props.theme.colors.grey1};
@@ -17766,330 +20507,330 @@
     function whitespace(thing) {
         return typeof thing === "object" ? thing.type === "text" ? empty$3(thing.value) : false : empty$3(thing);
     }
 
     function empty$3(value) {
         return value.replace(re$1, "") === "";
     }
-    class Schema {
+    class Schema$1 {
         constructor(property, normal, space2) {
             this.property = property;
             this.normal = normal;
             if (space2) {
                 this.space = space2;
             }
         }
     }
-    Schema.prototype.property = {};
-    Schema.prototype.normal = {};
-    Schema.prototype.space = null;
+    Schema$1.prototype.property = {};
+    Schema$1.prototype.normal = {};
+    Schema$1.prototype.space = null;
 
-    function merge$1(definitions, space2) {
+    function merge$2(definitions, space2) {
         const property = {};
         const normal = {};
         let index2 = -1;
         while (++index2 < definitions.length) {
             Object.assign(property, definitions[index2].property);
             Object.assign(normal, definitions[index2].normal);
         }
-        return new Schema(property, normal, space2);
+        return new Schema$1(property, normal, space2);
     }
 
-    function normalize$2(value) {
+    function normalize$3(value) {
         return value.toLowerCase();
     }
-    class Info {
+    class Info$1 {
         constructor(property, attribute) {
             this.property = property;
             this.attribute = attribute;
         }
     }
-    Info.prototype.space = null;
-    Info.prototype.boolean = false;
-    Info.prototype.booleanish = false;
-    Info.prototype.overloadedBoolean = false;
-    Info.prototype.number = false;
-    Info.prototype.commaSeparated = false;
-    Info.prototype.spaceSeparated = false;
-    Info.prototype.commaOrSpaceSeparated = false;
-    Info.prototype.mustUseProperty = false;
-    Info.prototype.defined = false;
-    let powers = 0;
-    const boolean = increment();
-    const booleanish = increment();
-    const overloadedBoolean = increment();
-    const number$3 = increment();
-    const spaceSeparated = increment();
-    const commaSeparated = increment();
-    const commaOrSpaceSeparated = increment();
+    Info$1.prototype.space = null;
+    Info$1.prototype.boolean = false;
+    Info$1.prototype.booleanish = false;
+    Info$1.prototype.overloadedBoolean = false;
+    Info$1.prototype.number = false;
+    Info$1.prototype.commaSeparated = false;
+    Info$1.prototype.spaceSeparated = false;
+    Info$1.prototype.commaOrSpaceSeparated = false;
+    Info$1.prototype.mustUseProperty = false;
+    Info$1.prototype.defined = false;
+    let powers$1 = 0;
+    const boolean$1 = increment$1();
+    const booleanish$1 = increment$1();
+    const overloadedBoolean$1 = increment$1();
+    const number$4 = increment$1();
+    const spaceSeparated$1 = increment$1();
+    const commaSeparated$1 = increment$1();
+    const commaOrSpaceSeparated$1 = increment$1();
 
-    function increment() {
-        return 2 ** ++powers;
+    function increment$1() {
+        return 2 ** ++powers$1;
     }
-    const types$1 = /* @__PURE__ */ Object.freeze( /* @__PURE__ */ Object.defineProperty({
+    const types$2 = /* @__PURE__ */ Object.freeze( /* @__PURE__ */ Object.defineProperty({
         __proto__: null,
-        boolean,
-        booleanish,
-        overloadedBoolean,
-        number: number$3,
-        spaceSeparated,
-        commaSeparated,
-        commaOrSpaceSeparated
+        boolean: boolean$1,
+        booleanish: booleanish$1,
+        overloadedBoolean: overloadedBoolean$1,
+        number: number$4,
+        spaceSeparated: spaceSeparated$1,
+        commaSeparated: commaSeparated$1,
+        commaOrSpaceSeparated: commaOrSpaceSeparated$1
     }, Symbol.toStringTag, {
         value: "Module"
     }));
-    const checks = Object.keys(types$1);
-    class DefinedInfo extends Info {
+    const checks$1 = Object.keys(types$2);
+    class DefinedInfo$1 extends Info$1 {
         constructor(property, attribute, mask, space2) {
             let index2 = -1;
             super(property, attribute);
-            mark(this, "space", space2);
+            mark$1(this, "space", space2);
             if (typeof mask === "number") {
-                while (++index2 < checks.length) {
-                    const check = checks[index2];
-                    mark(this, checks[index2], (mask & types$1[check]) === types$1[check]);
+                while (++index2 < checks$1.length) {
+                    const check = checks$1[index2];
+                    mark$1(this, checks$1[index2], (mask & types$2[check]) === types$2[check]);
                 }
             }
         }
     }
-    DefinedInfo.prototype.defined = true;
+    DefinedInfo$1.prototype.defined = true;
 
-    function mark(values, key, value) {
+    function mark$1(values, key, value) {
         if (value) {
             values[key] = value;
         }
     }
-    const own$8 = {}.hasOwnProperty;
+    const own$9 = {}.hasOwnProperty;
 
-    function create$1(definition2) {
+    function create$2(definition2) {
         const property = {};
         const normal = {};
         let prop;
         for (prop in definition2.properties) {
-            if (own$8.call(definition2.properties, prop)) {
+            if (own$9.call(definition2.properties, prop)) {
                 const value = definition2.properties[prop];
-                const info = new DefinedInfo(
+                const info = new DefinedInfo$1(
                     prop,
                     definition2.transform(definition2.attributes || {}, prop),
                     value,
                     definition2.space
                 );
                 if (definition2.mustUseProperty && definition2.mustUseProperty.includes(prop)) {
                     info.mustUseProperty = true;
                 }
                 property[prop] = info;
-                normal[normalize$2(prop)] = prop;
-                normal[normalize$2(info.attribute)] = prop;
+                normal[normalize$3(prop)] = prop;
+                normal[normalize$3(info.attribute)] = prop;
             }
         }
-        return new Schema(property, normal, definition2.space);
+        return new Schema$1(property, normal, definition2.space);
     }
-    const xlink = create$1({
+    const xlink$1 = create$2({
         space: "xlink",
         transform(_2, prop) {
             return "xlink:" + prop.slice(5).toLowerCase();
         },
         properties: {
             xLinkActuate: null,
             xLinkArcRole: null,
             xLinkHref: null,
             xLinkRole: null,
             xLinkShow: null,
             xLinkTitle: null,
             xLinkType: null
         }
     });
-    const xml = create$1({
+    const xml$1 = create$2({
         space: "xml",
         transform(_2, prop) {
             return "xml:" + prop.slice(3).toLowerCase();
         },
         properties: {
             xmlLang: null,
             xmlBase: null,
             xmlSpace: null
         }
     });
 
-    function caseSensitiveTransform(attributes2, attribute) {
+    function caseSensitiveTransform$1(attributes2, attribute) {
         return attribute in attributes2 ? attributes2[attribute] : attribute;
     }
 
-    function caseInsensitiveTransform(attributes2, property) {
-        return caseSensitiveTransform(attributes2, property.toLowerCase());
+    function caseInsensitiveTransform$1(attributes2, property) {
+        return caseSensitiveTransform$1(attributes2, property.toLowerCase());
     }
-    const xmlns = create$1({
+    const xmlns$1 = create$2({
         space: "xmlns",
         attributes: {
             xmlnsxlink: "xmlns:xlink"
         },
-        transform: caseInsensitiveTransform,
+        transform: caseInsensitiveTransform$1,
         properties: {
             xmlns: null,
             xmlnsXLink: null
         }
     });
-    const aria = create$1({
+    const aria$1 = create$2({
         transform(_2, prop) {
             return prop === "role" ? prop : "aria-" + prop.slice(4).toLowerCase();
         },
         properties: {
             ariaActiveDescendant: null,
-            ariaAtomic: booleanish,
+            ariaAtomic: booleanish$1,
             ariaAutoComplete: null,
-            ariaBusy: booleanish,
-            ariaChecked: booleanish,
-            ariaColCount: number$3,
-            ariaColIndex: number$3,
-            ariaColSpan: number$3,
-            ariaControls: spaceSeparated,
+            ariaBusy: booleanish$1,
+            ariaChecked: booleanish$1,
+            ariaColCount: number$4,
+            ariaColIndex: number$4,
+            ariaColSpan: number$4,
+            ariaControls: spaceSeparated$1,
             ariaCurrent: null,
-            ariaDescribedBy: spaceSeparated,
+            ariaDescribedBy: spaceSeparated$1,
             ariaDetails: null,
-            ariaDisabled: booleanish,
-            ariaDropEffect: spaceSeparated,
+            ariaDisabled: booleanish$1,
+            ariaDropEffect: spaceSeparated$1,
             ariaErrorMessage: null,
-            ariaExpanded: booleanish,
-            ariaFlowTo: spaceSeparated,
-            ariaGrabbed: booleanish,
+            ariaExpanded: booleanish$1,
+            ariaFlowTo: spaceSeparated$1,
+            ariaGrabbed: booleanish$1,
             ariaHasPopup: null,
-            ariaHidden: booleanish,
+            ariaHidden: booleanish$1,
             ariaInvalid: null,
             ariaKeyShortcuts: null,
             ariaLabel: null,
-            ariaLabelledBy: spaceSeparated,
-            ariaLevel: number$3,
+            ariaLabelledBy: spaceSeparated$1,
+            ariaLevel: number$4,
             ariaLive: null,
-            ariaModal: booleanish,
-            ariaMultiLine: booleanish,
-            ariaMultiSelectable: booleanish,
+            ariaModal: booleanish$1,
+            ariaMultiLine: booleanish$1,
+            ariaMultiSelectable: booleanish$1,
             ariaOrientation: null,
-            ariaOwns: spaceSeparated,
+            ariaOwns: spaceSeparated$1,
             ariaPlaceholder: null,
-            ariaPosInSet: number$3,
-            ariaPressed: booleanish,
-            ariaReadOnly: booleanish,
+            ariaPosInSet: number$4,
+            ariaPressed: booleanish$1,
+            ariaReadOnly: booleanish$1,
             ariaRelevant: null,
-            ariaRequired: booleanish,
-            ariaRoleDescription: spaceSeparated,
-            ariaRowCount: number$3,
-            ariaRowIndex: number$3,
-            ariaRowSpan: number$3,
-            ariaSelected: booleanish,
-            ariaSetSize: number$3,
+            ariaRequired: booleanish$1,
+            ariaRoleDescription: spaceSeparated$1,
+            ariaRowCount: number$4,
+            ariaRowIndex: number$4,
+            ariaRowSpan: number$4,
+            ariaSelected: booleanish$1,
+            ariaSetSize: number$4,
             ariaSort: null,
-            ariaValueMax: number$3,
-            ariaValueMin: number$3,
-            ariaValueNow: number$3,
+            ariaValueMax: number$4,
+            ariaValueMin: number$4,
+            ariaValueNow: number$4,
             ariaValueText: null,
             role: null
         }
     });
-    const html$4 = create$1({
+    const html$6 = create$2({
         space: "html",
         attributes: {
             acceptcharset: "accept-charset",
             classname: "class",
             htmlfor: "for",
             httpequiv: "http-equiv"
         },
-        transform: caseInsensitiveTransform,
+        transform: caseInsensitiveTransform$1,
         mustUseProperty: ["checked", "multiple", "muted", "selected"],
         properties: {
             abbr: null,
-            accept: commaSeparated,
-            acceptCharset: spaceSeparated,
-            accessKey: spaceSeparated,
+            accept: commaSeparated$1,
+            acceptCharset: spaceSeparated$1,
+            accessKey: spaceSeparated$1,
             action: null,
             allow: null,
-            allowFullScreen: boolean,
-            allowPaymentRequest: boolean,
-            allowUserMedia: boolean,
+            allowFullScreen: boolean$1,
+            allowPaymentRequest: boolean$1,
+            allowUserMedia: boolean$1,
             alt: null,
             as: null,
-            async: boolean,
+            async: boolean$1,
             autoCapitalize: null,
-            autoComplete: spaceSeparated,
-            autoFocus: boolean,
-            autoPlay: boolean,
-            blocking: spaceSeparated,
-            capture: boolean,
+            autoComplete: spaceSeparated$1,
+            autoFocus: boolean$1,
+            autoPlay: boolean$1,
+            blocking: spaceSeparated$1,
+            capture: null,
             charSet: null,
-            checked: boolean,
+            checked: boolean$1,
             cite: null,
-            className: spaceSeparated,
-            cols: number$3,
+            className: spaceSeparated$1,
+            cols: number$4,
             colSpan: null,
             content: null,
-            contentEditable: booleanish,
-            controls: boolean,
-            controlsList: spaceSeparated,
-            coords: number$3 | commaSeparated,
+            contentEditable: booleanish$1,
+            controls: boolean$1,
+            controlsList: spaceSeparated$1,
+            coords: number$4 | commaSeparated$1,
             crossOrigin: null,
             data: null,
             dateTime: null,
             decoding: null,
-            default: boolean,
-            defer: boolean,
+            default: boolean$1,
+            defer: boolean$1,
             dir: null,
             dirName: null,
-            disabled: boolean,
-            download: overloadedBoolean,
-            draggable: booleanish,
+            disabled: boolean$1,
+            download: overloadedBoolean$1,
+            draggable: booleanish$1,
             encType: null,
             enterKeyHint: null,
             fetchPriority: null,
             form: null,
             formAction: null,
             formEncType: null,
             formMethod: null,
-            formNoValidate: boolean,
+            formNoValidate: boolean$1,
             formTarget: null,
-            headers: spaceSeparated,
-            height: number$3,
-            hidden: boolean,
-            high: number$3,
+            headers: spaceSeparated$1,
+            height: number$4,
+            hidden: boolean$1,
+            high: number$4,
             href: null,
             hrefLang: null,
-            htmlFor: spaceSeparated,
-            httpEquiv: spaceSeparated,
+            htmlFor: spaceSeparated$1,
+            httpEquiv: spaceSeparated$1,
             id: null,
             imageSizes: null,
             imageSrcSet: null,
-            inert: boolean,
+            inert: boolean$1,
             inputMode: null,
             integrity: null,
             is: null,
-            isMap: boolean,
+            isMap: boolean$1,
             itemId: null,
-            itemProp: spaceSeparated,
-            itemRef: spaceSeparated,
-            itemScope: boolean,
-            itemType: spaceSeparated,
+            itemProp: spaceSeparated$1,
+            itemRef: spaceSeparated$1,
+            itemScope: boolean$1,
+            itemType: spaceSeparated$1,
             kind: null,
             label: null,
             lang: null,
             language: null,
             list: null,
             loading: null,
-            loop: boolean,
-            low: number$3,
+            loop: boolean$1,
+            low: number$4,
             manifest: null,
             max: null,
-            maxLength: number$3,
+            maxLength: number$4,
             media: null,
             method: null,
             min: null,
-            minLength: number$3,
-            multiple: boolean,
-            muted: boolean,
+            minLength: number$4,
+            multiple: boolean$1,
+            muted: boolean$1,
             name: null,
             nonce: null,
-            noModule: boolean,
-            noValidate: boolean,
+            noModule: boolean$1,
+            noValidate: boolean$1,
             onAbort: null,
             onAfterPrint: null,
             onAuxClick: null,
             onBeforeMatch: null,
             onBeforePrint: null,
             onBeforeToggle: null,
             onBeforeUnload: null,
@@ -18170,128 +20911,130 @@
             onTimeUpdate: null,
             onToggle: null,
             onUnhandledRejection: null,
             onUnload: null,
             onVolumeChange: null,
             onWaiting: null,
             onWheel: null,
-            open: boolean,
-            optimum: number$3,
+            open: boolean$1,
+            optimum: number$4,
             pattern: null,
-            ping: spaceSeparated,
+            ping: spaceSeparated$1,
             placeholder: null,
-            playsInline: boolean,
+            playsInline: boolean$1,
             popover: null,
             popoverTarget: null,
             popoverTargetAction: null,
             poster: null,
             preload: null,
-            readOnly: boolean,
+            readOnly: boolean$1,
             referrerPolicy: null,
-            rel: spaceSeparated,
-            required: boolean,
-            reversed: boolean,
-            rows: number$3,
-            rowSpan: number$3,
-            sandbox: spaceSeparated,
+            rel: spaceSeparated$1,
+            required: boolean$1,
+            reversed: boolean$1,
+            rows: number$4,
+            rowSpan: number$4,
+            sandbox: spaceSeparated$1,
             scope: null,
-            scoped: boolean,
-            seamless: boolean,
-            selected: boolean,
-            shadowRootDelegatesFocus: boolean,
+            scoped: boolean$1,
+            seamless: boolean$1,
+            selected: boolean$1,
+            shadowRootClonable: boolean$1,
+            shadowRootDelegatesFocus: boolean$1,
             shadowRootMode: null,
             shape: null,
-            size: number$3,
+            size: number$4,
             sizes: null,
             slot: null,
-            span: number$3,
-            spellCheck: booleanish,
+            span: number$4,
+            spellCheck: booleanish$1,
             src: null,
             srcDoc: null,
             srcLang: null,
             srcSet: null,
-            start: number$3,
+            start: number$4,
             step: null,
             style: null,
-            tabIndex: number$3,
+            tabIndex: number$4,
             target: null,
             title: null,
             translate: null,
             type: null,
-            typeMustMatch: boolean,
+            typeMustMatch: boolean$1,
             useMap: null,
-            value: booleanish,
-            width: number$3,
+            value: booleanish$1,
+            width: number$4,
             wrap: null,
+            writingSuggestions: null,
             align: null,
             aLink: null,
-            archive: spaceSeparated,
+            archive: spaceSeparated$1,
             axis: null,
             background: null,
             bgColor: null,
-            border: number$3,
+            border: number$4,
             borderColor: null,
-            bottomMargin: number$3,
+            bottomMargin: number$4,
             cellPadding: null,
             cellSpacing: null,
             char: null,
             charOff: null,
             classId: null,
             clear: null,
             code: null,
             codeBase: null,
             codeType: null,
             color: null,
-            compact: boolean,
-            declare: boolean,
+            compact: boolean$1,
+            declare: boolean$1,
             event: null,
             face: null,
             frame: null,
             frameBorder: null,
-            hSpace: number$3,
-            leftMargin: number$3,
+            hSpace: number$4,
+            leftMargin: number$4,
             link: null,
             longDesc: null,
             lowSrc: null,
-            marginHeight: number$3,
-            marginWidth: number$3,
-            noResize: boolean,
-            noHref: boolean,
-            noShade: boolean,
-            noWrap: boolean,
+            marginHeight: number$4,
+            marginWidth: number$4,
+            noResize: boolean$1,
+            noHref: boolean$1,
+            noShade: boolean$1,
+            noWrap: boolean$1,
             object: null,
             profile: null,
             prompt: null,
             rev: null,
-            rightMargin: number$3,
+            rightMargin: number$4,
             rules: null,
             scheme: null,
-            scrolling: booleanish,
+            scrolling: booleanish$1,
             standby: null,
             summary: null,
             text: null,
-            topMargin: number$3,
+            topMargin: number$4,
             valueType: null,
             version: null,
             vAlign: null,
             vLink: null,
-            vSpace: number$3,
+            vSpace: number$4,
             allowTransparency: null,
             autoCorrect: null,
             autoSave: null,
-            disablePictureInPicture: boolean,
-            disableRemotePlayback: boolean,
+            disablePictureInPicture: boolean$1,
+            disableRemotePlayback: boolean$1,
             prefix: null,
             property: null,
-            results: number$3,
+            results: number$4,
             security: null,
             unselectable: null
         }
     });
-    const svg$1 = create$1({
+    const svg$3 = create$2({
         space: "svg",
         attributes: {
             accentHeight: "accent-height",
             alignmentBaseline: "alignment-baseline",
             arabicForm: "arabic-form",
             baselineShift: "baseline-shift",
             capHeight: "cap-height",
@@ -18459,39 +21202,39 @@
             vertOriginY: "vert-origin-y",
             wordSpacing: "word-spacing",
             writingMode: "writing-mode",
             xHeight: "x-height",
             playbackOrder: "playbackorder",
             timelineBegin: "timelinebegin"
         },
-        transform: caseSensitiveTransform,
+        transform: caseSensitiveTransform$1,
         properties: {
-            about: commaOrSpaceSeparated,
-            accentHeight: number$3,
+            about: commaOrSpaceSeparated$1,
+            accentHeight: number$4,
             accumulate: null,
             additive: null,
             alignmentBaseline: null,
-            alphabetic: number$3,
-            amplitude: number$3,
+            alphabetic: number$4,
+            amplitude: number$4,
             arabicForm: null,
-            ascent: number$3,
+            ascent: number$4,
             attributeName: null,
             attributeType: null,
-            azimuth: number$3,
+            azimuth: number$4,
             bandwidth: null,
             baselineShift: null,
             baseFrequency: null,
             baseProfile: null,
             bbox: null,
             begin: null,
-            bias: number$3,
+            bias: number$4,
             by: null,
             calcMode: null,
-            capHeight: number$3,
-            className: spaceSeparated,
+            capHeight: number$4,
+            className: spaceSeparated$1,
             clip: null,
             clipPath: null,
             clipPathUnits: null,
             clipRule: null,
             color: null,
             colorInterpolation: null,
             colorInterpolationFilters: null,
@@ -18503,34 +21246,34 @@
             crossOrigin: null,
             cursor: null,
             cx: null,
             cy: null,
             d: null,
             dataType: null,
             defaultAction: null,
-            descent: number$3,
-            diffuseConstant: number$3,
+            descent: number$4,
+            diffuseConstant: number$4,
             direction: null,
             display: null,
             dur: null,
-            divisor: number$3,
+            divisor: number$4,
             dominantBaseline: null,
-            download: boolean,
+            download: boolean$1,
             dx: null,
             dy: null,
             edgeMode: null,
             editable: null,
-            elevation: number$3,
+            elevation: number$4,
             enableBackground: null,
             end: null,
             event: null,
-            exponent: number$3,
+            exponent: number$4,
             externalResourcesRequired: null,
             fill: null,
-            fillOpacity: number$3,
+            fillOpacity: number$4,
             fillRule: null,
             filter: null,
             filterRes: null,
             filterUnits: null,
             floodColor: null,
             floodOpacity: null,
             focusable: null,
@@ -18543,55 +21286,55 @@
             fontVariant: null,
             fontWeight: null,
             format: null,
             fr: null,
             from: null,
             fx: null,
             fy: null,
-            g1: commaSeparated,
-            g2: commaSeparated,
-            glyphName: commaSeparated,
+            g1: commaSeparated$1,
+            g2: commaSeparated$1,
+            glyphName: commaSeparated$1,
             glyphOrientationHorizontal: null,
             glyphOrientationVertical: null,
             glyphRef: null,
             gradientTransform: null,
             gradientUnits: null,
             handler: null,
-            hanging: number$3,
+            hanging: number$4,
             hatchContentUnits: null,
             hatchUnits: null,
             height: null,
             href: null,
             hrefLang: null,
-            horizAdvX: number$3,
-            horizOriginX: number$3,
-            horizOriginY: number$3,
+            horizAdvX: number$4,
+            horizOriginX: number$4,
+            horizOriginY: number$4,
             id: null,
-            ideographic: number$3,
+            ideographic: number$4,
             imageRendering: null,
             initialVisibility: null,
             in: null,
             in2: null,
-            intercept: number$3,
-            k: number$3,
-            k1: number$3,
-            k2: number$3,
-            k3: number$3,
-            k4: number$3,
-            kernelMatrix: commaOrSpaceSeparated,
+            intercept: number$4,
+            k: number$4,
+            k1: number$4,
+            k2: number$4,
+            k3: number$4,
+            k4: number$4,
+            kernelMatrix: commaOrSpaceSeparated$1,
             kernelUnitLength: null,
             keyPoints: null,
             keySplines: null,
             keyTimes: null,
             kerning: null,
             lang: null,
             lengthAdjust: null,
             letterSpacing: null,
             lightingColor: null,
-            limitingConeAngle: number$3,
+            limitingConeAngle: number$4,
             local: null,
             markerEnd: null,
             markerMid: null,
             markerStart: null,
             markerHeight: null,
             markerUnits: null,
             markerWidth: null,
@@ -18599,15 +21342,15 @@
             maskContentUnits: null,
             maskUnits: null,
             mathematical: null,
             max: null,
             media: null,
             mediaCharacterEncoding: null,
             mediaContentEncodings: null,
-            mediaSize: number$3,
+            mediaSize: number$4,
             mediaTime: null,
             method: null,
             min: null,
             mode: null,
             name: null,
             navDown: null,
             navDownLeft: null,
@@ -18705,183 +21448,183 @@
             operator: null,
             order: null,
             orient: null,
             orientation: null,
             origin: null,
             overflow: null,
             overlay: null,
-            overlinePosition: number$3,
-            overlineThickness: number$3,
+            overlinePosition: number$4,
+            overlineThickness: number$4,
             paintOrder: null,
             panose1: null,
             path: null,
-            pathLength: number$3,
+            pathLength: number$4,
             patternContentUnits: null,
             patternTransform: null,
             patternUnits: null,
             phase: null,
-            ping: spaceSeparated,
+            ping: spaceSeparated$1,
             pitch: null,
             playbackOrder: null,
             pointerEvents: null,
             points: null,
-            pointsAtX: number$3,
-            pointsAtY: number$3,
-            pointsAtZ: number$3,
+            pointsAtX: number$4,
+            pointsAtY: number$4,
+            pointsAtZ: number$4,
             preserveAlpha: null,
             preserveAspectRatio: null,
             primitiveUnits: null,
             propagate: null,
-            property: commaOrSpaceSeparated,
+            property: commaOrSpaceSeparated$1,
             r: null,
             radius: null,
             referrerPolicy: null,
             refX: null,
             refY: null,
-            rel: commaOrSpaceSeparated,
-            rev: commaOrSpaceSeparated,
+            rel: commaOrSpaceSeparated$1,
+            rev: commaOrSpaceSeparated$1,
             renderingIntent: null,
             repeatCount: null,
             repeatDur: null,
-            requiredExtensions: commaOrSpaceSeparated,
-            requiredFeatures: commaOrSpaceSeparated,
-            requiredFonts: commaOrSpaceSeparated,
-            requiredFormats: commaOrSpaceSeparated,
+            requiredExtensions: commaOrSpaceSeparated$1,
+            requiredFeatures: commaOrSpaceSeparated$1,
+            requiredFonts: commaOrSpaceSeparated$1,
+            requiredFormats: commaOrSpaceSeparated$1,
             resource: null,
             restart: null,
             result: null,
             rotate: null,
             rx: null,
             ry: null,
             scale: null,
             seed: null,
             shapeRendering: null,
             side: null,
             slope: null,
             snapshotTime: null,
-            specularConstant: number$3,
-            specularExponent: number$3,
+            specularConstant: number$4,
+            specularExponent: number$4,
             spreadMethod: null,
             spacing: null,
             startOffset: null,
             stdDeviation: null,
             stemh: null,
             stemv: null,
             stitchTiles: null,
             stopColor: null,
             stopOpacity: null,
-            strikethroughPosition: number$3,
-            strikethroughThickness: number$3,
+            strikethroughPosition: number$4,
+            strikethroughThickness: number$4,
             string: null,
             stroke: null,
-            strokeDashArray: commaOrSpaceSeparated,
+            strokeDashArray: commaOrSpaceSeparated$1,
             strokeDashOffset: null,
             strokeLineCap: null,
             strokeLineJoin: null,
-            strokeMiterLimit: number$3,
-            strokeOpacity: number$3,
+            strokeMiterLimit: number$4,
+            strokeOpacity: number$4,
             strokeWidth: null,
             style: null,
-            surfaceScale: number$3,
+            surfaceScale: number$4,
             syncBehavior: null,
             syncBehaviorDefault: null,
             syncMaster: null,
             syncTolerance: null,
             syncToleranceDefault: null,
-            systemLanguage: commaOrSpaceSeparated,
-            tabIndex: number$3,
+            systemLanguage: commaOrSpaceSeparated$1,
+            tabIndex: number$4,
             tableValues: null,
             target: null,
-            targetX: number$3,
-            targetY: number$3,
+            targetX: number$4,
+            targetY: number$4,
             textAnchor: null,
             textDecoration: null,
             textRendering: null,
             textLength: null,
             timelineBegin: null,
             title: null,
             transformBehavior: null,
             type: null,
-            typeOf: commaOrSpaceSeparated,
+            typeOf: commaOrSpaceSeparated$1,
             to: null,
             transform: null,
             transformOrigin: null,
             u1: null,
             u2: null,
-            underlinePosition: number$3,
-            underlineThickness: number$3,
+            underlinePosition: number$4,
+            underlineThickness: number$4,
             unicode: null,
             unicodeBidi: null,
             unicodeRange: null,
-            unitsPerEm: number$3,
+            unitsPerEm: number$4,
             values: null,
-            vAlphabetic: number$3,
-            vMathematical: number$3,
+            vAlphabetic: number$4,
+            vMathematical: number$4,
             vectorEffect: null,
-            vHanging: number$3,
-            vIdeographic: number$3,
+            vHanging: number$4,
+            vIdeographic: number$4,
             version: null,
-            vertAdvY: number$3,
-            vertOriginX: number$3,
-            vertOriginY: number$3,
+            vertAdvY: number$4,
+            vertOriginX: number$4,
+            vertOriginY: number$4,
             viewBox: null,
             viewTarget: null,
             visibility: null,
             width: null,
             widths: null,
             wordSpacing: null,
             writingMode: null,
             x: null,
             x1: null,
             x2: null,
             xChannelSelector: null,
-            xHeight: number$3,
+            xHeight: number$4,
             y: null,
             y1: null,
             y2: null,
             yChannelSelector: null,
             z: null,
             zoomAndPan: null
         }
     });
-    const valid$1 = /^data[-\w.:]+$/i;
-    const dash = /-[a-z]/g;
-    const cap$1 = /[A-Z]/g;
+    const valid$2 = /^data[-\w.:]+$/i;
+    const dash$1 = /-[a-z]/g;
+    const cap$2 = /[A-Z]/g;
 
-    function find$3(schema, value) {
-        const normal = normalize$2(value);
+    function find$4(schema, value) {
+        const normal = normalize$3(value);
         let prop = value;
-        let Type2 = Info;
+        let Type2 = Info$1;
         if (normal in schema.normal) {
             return schema.property[schema.normal[normal]];
         }
-        if (normal.length > 4 && normal.slice(0, 4) === "data" && valid$1.test(value)) {
+        if (normal.length > 4 && normal.slice(0, 4) === "data" && valid$2.test(value)) {
             if (value.charAt(4) === "-") {
-                const rest = value.slice(5).replace(dash, camelcase);
+                const rest = value.slice(5).replace(dash$1, camelcase$1);
                 prop = "data" + rest.charAt(0).toUpperCase() + rest.slice(1);
             } else {
                 const rest = value.slice(4);
-                if (!dash.test(rest)) {
-                    let dashes = rest.replace(cap$1, kebab);
+                if (!dash$1.test(rest)) {
+                    let dashes = rest.replace(cap$2, kebab$1);
                     if (dashes.charAt(0) !== "-") {
                         dashes = "-" + dashes;
                     }
                     value = "data" + dashes;
                 }
             }
-            Type2 = DefinedInfo;
+            Type2 = DefinedInfo$1;
         }
         return new Type2(prop, value);
     }
 
-    function kebab($0) {
+    function kebab$1($0) {
         return "-" + $0.toLowerCase();
     }
 
-    function camelcase($0) {
+    function camelcase$1($0) {
         return $0.charAt(1).toUpperCase();
     }
     const hastToReact = {
         classId: "classID",
         dataType: "datatype",
         itemId: "itemID",
         strokeDashArray: "strokeDasharray",
@@ -18895,16 +21638,16 @@
         xLinkHref: "xlinkHref",
         xLinkRole: "xlinkRole",
         xLinkShow: "xlinkShow",
         xLinkTitle: "xlinkTitle",
         xLinkType: "xlinkType",
         xmlnsXLink: "xmlnsXlink"
     };
-    const html$3 = merge$1([xml, xlink, xmlns, aria, html$4], "html");
-    const svg = merge$1([xml, xlink, xmlns, aria, svg$1], "svg");
+    const html$5 = merge$2([xml$1, xlink$1, xmlns$1, aria$1, html$6], "html");
+    const svg$2 = merge$2([xml$1, xlink$1, xmlns$1, aria$1, svg$3], "svg");
 
     function parse$7(value) {
         const input = String(value || "").trim();
         return input ? input.split(/[ \t\n\r\f]+/g) : [];
     }
 
     function stringify$2(values) {
@@ -19142,22 +21885,22 @@
         if ("line" in value || "column" in value) {
             return point$3(value);
         }
         return "";
     }
 
     function point$3(point2) {
-        return index$4(point2 && point2.line) + ":" + index$4(point2 && point2.column);
+        return index$2(point2 && point2.line) + ":" + index$2(point2 && point2.column);
     }
 
     function position$2(pos) {
         return point$3(pos && pos.start) + "-" + point$3(pos && pos.end);
     }
 
-    function index$4(value) {
+    function index$2(value) {
         return value && typeof value === "number" ? value : 1;
     }
     class VFileMessage extends Error {
         constructor(causeOrReason, optionsOrParentOrPlace, origin) {
             super();
             if (typeof optionsOrParentOrPlace === "string") {
                 origin = optionsOrParentOrPlace;
@@ -19237,17 +21980,17 @@
     VFileMessage.prototype.line = void 0;
     VFileMessage.prototype.ancestors = void 0;
     VFileMessage.prototype.cause = void 0;
     VFileMessage.prototype.fatal = void 0;
     VFileMessage.prototype.place = void 0;
     VFileMessage.prototype.ruleId = void 0;
     VFileMessage.prototype.source = void 0;
-    const own$7 = {}.hasOwnProperty;
+    const own$8 = {}.hasOwnProperty;
     const emptyMap = /* @__PURE__ */ new Map();
-    const cap = /[A-Z]/g;
+    const cap$1 = /[A-Z]/g;
     const dashSomething = /-([a-z])/g;
     const tableElements = /* @__PURE__ */ new Set(["table", "tbody", "thead", "tfoot", "tr"]);
     const tableCellElement = /* @__PURE__ */ new Set(["td", "th"]);
     const docs = "https://github.com/syntax-tree/hast-util-to-jsx-runtime";
 
     function toJsxRuntime(tree, options) {
         if (!options || options.Fragment === void 0) {
@@ -19278,15 +22021,15 @@
             create: create2,
             elementAttributeNameCase: options.elementAttributeNameCase || "react",
             evaluater: options.createEvaluater ? options.createEvaluater() : void 0,
             filePath,
             ignoreInvalidStyle: options.ignoreInvalidStyle || false,
             passKeys: options.passKeys !== false,
             passNode: options.passNode || false,
-            schema: options.space === "svg" ? svg : html$3,
+            schema: options.space === "svg" ? svg$2 : html$5,
             stylePropertyNameCase: options.stylePropertyNameCase || "dom",
             tableCellAlignToStyle: options.tableCellAlignToStyle !== false
         };
         const result = one$4(state, tree, void 0);
         if (result && typeof result !== "string") {
             return result;
         }
@@ -19320,15 +22063,15 @@
         }
     }
 
     function element$4(state, node2, key) {
         const parentSchema = state.schema;
         let schema = parentSchema;
         if (node2.tagName.toLowerCase() === "svg" && parentSchema.space === "html") {
-            schema = svg;
+            schema = svg$2;
             state.schema = schema;
         }
         state.ancestors.push(node2);
         const type2 = findComponentFromName(state, node2.tagName, false);
         const props = createElementProps(state, node2);
         let children2 = createChildren(state, node2);
         if (tableElements.has(node2.tagName)) {
@@ -19360,15 +22103,15 @@
         crashEstree(state, node2.position);
     }
 
     function mdxJsxElement(state, node2, key) {
         const parentSchema = state.schema;
         let schema = parentSchema;
         if (node2.name === "svg" && parentSchema.space === "html") {
-            schema = svg;
+            schema = svg$2;
             state.schema = schema;
         }
         state.ancestors.push(node2);
         const type2 = node2.name === null ? state.Fragment : findComponentFromName(state, node2.name, true);
         const props = createJsxElementProps(state, node2);
         const children2 = createChildren(state, node2);
         addNode$1(state, props, type2, node2);
@@ -19434,15 +22177,15 @@
     }
 
     function createElementProps(state, node2) {
         const props = {};
         let alignValue;
         let prop;
         for (prop in node2.properties) {
-            if (prop !== "children" && own$7.call(node2.properties, prop)) {
+            if (prop !== "children" && own$8.call(node2.properties, prop)) {
                 const result = createProperty$1(state, prop, node2.properties[prop]);
                 if (result) {
                     const [key, value] = result;
                     if (state.tableCellAlignToStyle && key === "align" && typeof value === "string" && tableCellElement.has(node2.tagName)) {
                         alignValue = value;
                     } else {
                         props[key] = value;
@@ -19516,15 +22259,15 @@
             if (result !== void 0)
                 children2.push(result);
         }
         return children2;
     }
 
     function createProperty$1(state, prop, value) {
-        const info = find$3(state.schema, prop);
+        const info = find$4(state.schema, prop);
         if (value === null || value === void 0 || typeof value === "number" && Number.isNaN(value)) {
             return;
         }
         if (Array.isArray(value)) {
             value = info.commaSeparated ? stringify$3(value) : stringify$2(value);
         }
         if (info.property === "style") {
@@ -19606,15 +22349,15 @@
             } : {
                 type: "Literal",
                 value: name2
             };
         }
         if (result.type === "Literal") {
             const name3 = result.value;
-            return own$7.call(state.components, name3) ? state.components[name3] : name3;
+            return own$8.call(state.components, name3) ? state.components[name3] : name3;
         }
         if (state.evaluater) {
             return state.evaluater.evaluateExpression(result);
         }
         crashEstree(state);
     }
 
@@ -19632,23 +22375,23 @@
         throw message;
     }
 
     function transformStylesToCssCasing(domCasing) {
         const cssCasing = {};
         let from;
         for (from in domCasing) {
-            if (own$7.call(domCasing, from)) {
+            if (own$8.call(domCasing, from)) {
                 cssCasing[transformStyleToCssCasing(from)] = domCasing[from];
             }
         }
         return cssCasing;
     }
 
     function transformStyleToCssCasing(from) {
-        let to2 = from.replace(cap, toDash);
+        let to2 = from.replace(cap$1, toDash);
         if (to2.slice(0, 3) === "ms-")
             to2 = "-" + to2;
         return to2;
     }
 
     function toCamel(_2, $1) {
         return $1.toUpperCase();
@@ -20267,22 +23010,15 @@
                         }
                         nextEvents = push$2(nextEvents, [
                             ["enter", group, context2],
                             ["enter", openingSequence, context2],
                             ["exit", openingSequence, context2],
                             ["enter", text2, context2]
                         ]);
-                        nextEvents = push$2(
-                            nextEvents,
-                            resolveAll(
-                                context2.parser.constructs.insideSpan.null,
-                                events2.slice(open + 1, index2),
-                                context2
-                            )
-                        );
+                        nextEvents = push$2(nextEvents, resolveAll(context2.parser.constructs.insideSpan.null, events2.slice(open + 1, index2), context2));
                         nextEvents = push$2(nextEvents, [
                             ["exit", text2, context2],
                             ["enter", closingSequence, context2],
                             ["exit", closingSequence, context2],
                             ["exit", group, context2]
                         ]);
                         if (events2[index2][1].end.offset - events2[index2][1].start.offset) {
@@ -20362,14 +23098,17 @@
         }
 
         function open(code2) {
             if (asciiAlpha(code2)) {
                 effects.consume(code2);
                 return schemeOrEmailAtext;
             }
+            if (code2 === 64) {
+                return nok(code2);
+            }
             return emailAtext(code2);
         }
 
         function schemeOrEmailAtext(code2) {
             if (code2 === 43 || code2 === 45 || code2 === 46 || asciiAlphanumeric(code2)) {
                 size2 = 1;
                 return schemeInsideOrEmailAtext(code2);
@@ -20511,20 +23250,15 @@
 
     function tokenizeBlockQuoteContinuation(effects, ok2, nok) {
         const self2 = this;
         return contStart;
 
         function contStart(code2) {
             if (markdownSpace(code2)) {
-                return factorySpace(
-                    effects,
-                    contBefore,
-                    "linePrefix",
-                    self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4
-                )(code2);
+                return factorySpace(effects, contBefore, "linePrefix", self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4)(code2);
             }
             return contBefore(code2);
         }
 
         function contBefore(code2) {
             return effects.attempt(blockQuote, ok2, nok)(code2);
         }
@@ -20738,20 +23472,15 @@
             effects.enter("lineEnding");
             effects.consume(code2);
             effects.exit("lineEnding");
             return contentStart;
         }
 
         function contentStart(code2) {
-            return initialPrefix > 0 && markdownSpace(code2) ? factorySpace(
-                effects,
-                beforeContentChunk,
-                "linePrefix",
-                initialPrefix + 1
-            )(code2) : beforeContentChunk(code2);
+            return initialPrefix > 0 && markdownSpace(code2) ? factorySpace(effects, beforeContentChunk, "linePrefix", initialPrefix + 1)(code2) : beforeContentChunk(code2);
         }
 
         function beforeContentChunk(code2) {
             if (code2 === null || markdownLineEnding(code2)) {
                 return effects.check(nonLazyContinuation, atNonLazyBreak, after)(code2);
             }
             effects.enter("codeFlowValue");
@@ -20781,20 +23510,15 @@
                 effects2.consume(code2);
                 effects2.exit("lineEnding");
                 return start3;
             }
 
             function start3(code2) {
                 effects2.enter("codeFencedFence");
-                return markdownSpace(code2) ? factorySpace(
-                    effects2,
-                    beforeSequenceClose,
-                    "linePrefix",
-                    self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4
-                )(code2) : beforeSequenceClose(code2);
+                return markdownSpace(code2) ? factorySpace(effects2, beforeSequenceClose, "linePrefix", self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4)(code2) : beforeSequenceClose(code2);
             }
 
             function beforeSequenceClose(code2) {
                 if (code2 === marker) {
                     effects2.enter("codeFencedFenceSequence");
                     return sequenceClose(code2);
                 }
@@ -21029,31 +23753,114 @@
                 effects.exit("codeText");
                 return ok2(code2);
             }
             token.type = "codeTextData";
             return data2(code2);
         }
     }
+    class SpliceBuffer {
+        constructor(initial2) {
+            this.left = initial2 ? [...initial2] : [];
+            this.right = [];
+        }
+        get(index2) {
+            if (index2 < 0 || index2 >= this.left.length + this.right.length) {
+                throw new RangeError("Cannot access index `" + index2 + "` in a splice buffer of size `" + (this.left.length + this.right.length) + "`");
+            }
+            if (index2 < this.left.length)
+                return this.left[index2];
+            return this.right[this.right.length - index2 + this.left.length - 1];
+        }
+        get length() {
+            return this.left.length + this.right.length;
+        }
+        shift() {
+            this.setCursor(0);
+            return this.right.pop();
+        }
+        slice(start2, end2) {
+            const stop = end2 === null || end2 === void 0 ? Number.POSITIVE_INFINITY : end2;
+            if (stop < this.left.length) {
+                return this.left.slice(start2, stop);
+            }
+            if (start2 > this.left.length) {
+                return this.right.slice(this.right.length - stop + this.left.length, this.right.length - start2 + this.left.length).reverse();
+            }
+            return this.left.slice(start2).concat(this.right.slice(this.right.length - stop + this.left.length).reverse());
+        }
+        splice(start2, deleteCount, items) {
+            const count2 = deleteCount || 0;
+            this.setCursor(Math.trunc(start2));
+            const removed = this.right.splice(this.right.length - count2, Number.POSITIVE_INFINITY);
+            if (items)
+                chunkedPush(this.left, items);
+            return removed.reverse();
+        }
+        pop() {
+            this.setCursor(Number.POSITIVE_INFINITY);
+            return this.left.pop();
+        }
+        push(item) {
+            this.setCursor(Number.POSITIVE_INFINITY);
+            this.left.push(item);
+        }
+        pushMany(items) {
+            this.setCursor(Number.POSITIVE_INFINITY);
+            chunkedPush(this.left, items);
+        }
+        unshift(item) {
+            this.setCursor(0);
+            this.right.push(item);
+        }
+        unshiftMany(items) {
+            this.setCursor(0);
+            chunkedPush(this.right, items.reverse());
+        }
+        setCursor(n2) {
+            if (n2 === this.left.length || n2 > this.left.length && this.right.length === 0 || n2 < 0 && this.left.length === 0)
+                return;
+            if (n2 < this.left.length) {
+                const removed = this.left.splice(n2, Number.POSITIVE_INFINITY);
+                chunkedPush(this.right, removed.reverse());
+            } else {
+                const removed = this.right.splice(this.left.length + this.right.length - n2, Number.POSITIVE_INFINITY);
+                chunkedPush(this.left, removed.reverse());
+            }
+        }
+    }
+
+    function chunkedPush(list2, right2) {
+        let chunkStart = 0;
+        if (right2.length < 1e4) {
+            list2.push(...right2);
+        } else {
+            while (chunkStart < right2.length) {
+                list2.push(...right2.slice(chunkStart, chunkStart + 1e4));
+                chunkStart += 1e4;
+            }
+        }
+    }
 
-    function subtokenize(events2) {
+    function subtokenize(eventsArray) {
         const jumps = {};
         let index2 = -1;
         let event2;
         let lineIndex;
         let otherIndex;
         let otherEvent;
         let parameters;
         let subevents;
         let more;
+        const events2 = new SpliceBuffer(eventsArray);
         while (++index2 < events2.length) {
             while (index2 in jumps) {
                 index2 = jumps[index2];
             }
-            event2 = events2[index2];
-            if (index2 && event2[1].type === "chunkFlow" && events2[index2 - 1][1].type === "listItemPrefix") {
+            event2 = events2.get(index2);
+            if (index2 && event2[1].type === "chunkFlow" && events2.get(index2 - 1)[1].type === "listItemPrefix") {
                 subevents = event2[1]._tokenizer.events;
                 otherIndex = 0;
                 if (otherIndex < subevents.length && subevents[otherIndex][1].type === "lineEndingBlank") {
                     otherIndex += 2;
                 }
                 if (otherIndex < subevents.length && subevents[otherIndex][1].type === "content") {
                     while (++otherIndex < subevents.length) {
@@ -21073,56 +23880,57 @@
                     index2 = jumps[index2];
                     more = true;
                 }
             } else if (event2[1]._container) {
                 otherIndex = index2;
                 lineIndex = void 0;
                 while (otherIndex--) {
-                    otherEvent = events2[otherIndex];
+                    otherEvent = events2.get(otherIndex);
                     if (otherEvent[1].type === "lineEnding" || otherEvent[1].type === "lineEndingBlank") {
                         if (otherEvent[0] === "enter") {
                             if (lineIndex) {
-                                events2[lineIndex][1].type = "lineEndingBlank";
+                                events2.get(lineIndex)[1].type = "lineEndingBlank";
                             }
                             otherEvent[1].type = "lineEnding";
                             lineIndex = otherIndex;
                         }
                     } else {
                         break;
                     }
                 }
                 if (lineIndex) {
-                    event2[1].end = Object.assign({}, events2[lineIndex][1].start);
+                    event2[1].end = Object.assign({}, events2.get(lineIndex)[1].start);
                     parameters = events2.slice(lineIndex, index2);
                     parameters.unshift(event2);
-                    splice$1(events2, lineIndex, index2 - lineIndex + 1, parameters);
+                    events2.splice(lineIndex, index2 - lineIndex + 1, parameters);
                 }
             }
         }
+        splice$1(eventsArray, 0, Number.POSITIVE_INFINITY, events2.slice(0));
         return !more;
     }
 
     function subcontent(events2, eventIndex) {
-        const token = events2[eventIndex][1];
-        const context2 = events2[eventIndex][2];
+        const token = events2.get(eventIndex)[1];
+        const context2 = events2.get(eventIndex)[2];
         let startPosition = eventIndex - 1;
         const startPositions = [];
         const tokenizer2 = token._tokenizer || context2.parser[token.contentType](token.start);
         const childEvents = tokenizer2.events;
         const jumps = [];
         const gaps = {};
         let stream;
         let previous2;
         let index2 = -1;
         let current2 = token;
         let adjust = 0;
         let start2 = 0;
         const breaks = [start2];
         while (current2) {
-            while (events2[++startPosition][1] !== current2) {}
+            while (events2.get(++startPosition)[1] !== current2) {}
             startPositions.push(startPosition);
             if (!current2._tokenizer) {
                 stream = context2.sliceStream(current2);
                 if (!current2.next) {
                     stream.push(null);
                 }
                 if (previous2) {
@@ -21156,17 +23964,18 @@
         } else {
             breaks.pop();
         }
         index2 = breaks.length;
         while (index2--) {
             const slice = childEvents.slice(breaks[index2], breaks[index2 + 1]);
             const start3 = startPositions.pop();
-            jumps.unshift([start3, start3 + slice.length - 1]);
-            splice$1(events2, start3, 2, slice);
+            jumps.push([start3, start3 + slice.length - 1]);
+            events2.splice(start3, 2, slice);
         }
+        jumps.reverse();
         index2 = -1;
         while (++index2 < jumps.length) {
             gaps[adjust + jumps[index2][0]] = adjust + jumps[index2][1];
             adjust += jumps[index2][1] - jumps[index2][0] - 1;
         }
         return gaps;
     }
@@ -21197,19 +24006,15 @@
         }
 
         function chunkInside(code2) {
             if (code2 === null) {
                 return contentEnd(code2);
             }
             if (markdownLineEnding(code2)) {
-                return effects.check(
-                    continuationConstruct,
-                    contentContinue,
-                    contentEnd
-                )(code2);
+                return effects.check(continuationConstruct, contentContinue, contentEnd)(code2);
             }
             effects.consume(code2);
             return chunkInside;
         }
 
         function contentEnd(code2) {
             effects.exit("chunkContent");
@@ -21526,17 +24331,15 @@
                 "definitionLabel",
                 "definitionLabelMarker",
                 "definitionLabelString"
             )(code2);
         }
 
         function labelAfter(code2) {
-            identifier = normalizeIdentifier(
-                self2.sliceSerialize(self2.events[self2.events.length - 1][1]).slice(1, -1)
-            );
+            identifier = normalizeIdentifier(self2.sliceSerialize(self2.events[self2.events.length - 1][1]).slice(1, -1));
             if (code2 === 58) {
                 effects.enter("definitionMarker");
                 effects.consume(code2);
                 effects.exit("definitionMarker");
                 return markerAfter;
             }
             return nok(code2);
@@ -21581,22 +24384,15 @@
         return titleBefore2;
 
         function titleBefore2(code2) {
             return markdownLineEndingOrSpace(code2) ? factoryWhitespace(effects, beforeMarker)(code2) : nok(code2);
         }
 
         function beforeMarker(code2) {
-            return factoryTitle(
-                effects,
-                titleAfter,
-                nok,
-                "definitionTitle",
-                "definitionTitleMarker",
-                "definitionTitleString"
-            )(code2);
+            return factoryTitle(effects, titleAfter, nok, "definitionTitle", "definitionTitleMarker", "definitionTitleString")(code2);
         }
 
         function titleAfter(code2) {
             return markdownSpace(code2) ? factorySpace(effects, titleAfterOptionalWhitespace, "whitespace")(code2) : titleAfterOptionalWhitespace(code2);
         }
 
         function titleAfterOptionalWhitespace(code2) {
@@ -22075,34 +24871,26 @@
             }
             if (code2 === 93 && marker === 5) {
                 effects.consume(code2);
                 return continuationCdataInside;
             }
             if (markdownLineEnding(code2) && (marker === 6 || marker === 7)) {
                 effects.exit("htmlFlowData");
-                return effects.check(
-                    blankLineBefore,
-                    continuationAfter,
-                    continuationStart
-                )(code2);
+                return effects.check(blankLineBefore, continuationAfter, continuationStart)(code2);
             }
             if (code2 === null || markdownLineEnding(code2)) {
                 effects.exit("htmlFlowData");
                 return continuationStart(code2);
             }
             effects.consume(code2);
             return continuation;
         }
 
         function continuationStart(code2) {
-            return effects.check(
-                nonLazyContinuationStart,
-                continuationStartNonLazy,
-                continuationAfter
-            )(code2);
+            return effects.check(nonLazyContinuationStart, continuationStartNonLazy, continuationAfter)(code2);
         }
 
         function continuationStartNonLazy(code2) {
             effects.enter("lineEnding");
             effects.consume(code2);
             effects.exit("lineEnding");
             return continuationBefore;
@@ -22536,20 +25324,15 @@
             effects.enter("lineEnding");
             effects.consume(code2);
             effects.exit("lineEnding");
             return lineEndingAfter;
         }
 
         function lineEndingAfter(code2) {
-            return markdownSpace(code2) ? factorySpace(
-                effects,
-                lineEndingAfterPrefix,
-                "linePrefix",
-                self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4
-            )(code2) : lineEndingAfterPrefix(code2);
+            return markdownSpace(code2) ? factorySpace(effects, lineEndingAfterPrefix, "linePrefix", self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4)(code2) : lineEndingAfterPrefix(code2);
         }
 
         function lineEndingAfterPrefix(code2) {
             effects.enter("htmlTextData");
             return returnState(code2);
         }
     }
@@ -22629,26 +25412,17 @@
             ["enter", group, context2],
             ["enter", label, context2]
         ];
         media = push$2(media, events2.slice(open + 1, open + offset2 + 3));
         media = push$2(media, [
             ["enter", text2, context2]
         ]);
-        media = push$2(
-            media,
-            resolveAll(
-                context2.parser.constructs.insideSpan.null,
-                events2.slice(open + offset2 + 4, close - 3),
-                context2
-            )
-        );
+        media = push$2(media, resolveAll(context2.parser.constructs.insideSpan.null, events2.slice(open + offset2 + 4, close - 3), context2));
         media = push$2(media, [
-            ["exit", text2, context2],
-            events2[close - 2],
-            events2[close - 1],
+            ["exit", text2, context2], events2[close - 2], events2[close - 1],
             ["exit", label, context2]
         ]);
         media = push$2(media, events2.slice(close + 1));
         media = push$2(media, [
             ["exit", group, context2]
         ]);
         splice$1(events2, open, events2.length, media);
@@ -22671,54 +25445,38 @@
         function start2(code2) {
             if (!labelStart) {
                 return nok(code2);
             }
             if (labelStart._inactive) {
                 return labelEndNok(code2);
             }
-            defined = self2.parser.defined.includes(
-                normalizeIdentifier(
-                    self2.sliceSerialize({
-                        start: labelStart.end,
-                        end: self2.now()
-                    })
-                )
-            );
+            defined = self2.parser.defined.includes(normalizeIdentifier(self2.sliceSerialize({
+                start: labelStart.end,
+                end: self2.now()
+            })));
             effects.enter("labelEnd");
             effects.enter("labelMarker");
             effects.consume(code2);
             effects.exit("labelMarker");
             effects.exit("labelEnd");
             return after;
         }
 
         function after(code2) {
             if (code2 === 40) {
-                return effects.attempt(
-                    resourceConstruct,
-                    labelEndOk,
-                    defined ? labelEndOk : labelEndNok
-                )(code2);
+                return effects.attempt(resourceConstruct, labelEndOk, defined ? labelEndOk : labelEndNok)(code2);
             }
             if (code2 === 91) {
-                return effects.attempt(
-                    referenceFullConstruct,
-                    labelEndOk,
-                    defined ? referenceNotFull : labelEndNok
-                )(code2);
+                return effects.attempt(referenceFullConstruct, labelEndOk, defined ? referenceNotFull : labelEndNok)(code2);
             }
             return defined ? labelEndOk(code2) : labelEndNok(code2);
         }
 
         function referenceNotFull(code2) {
-            return effects.attempt(
-                referenceCollapsedConstruct,
-                labelEndOk,
-                labelEndNok
-            )(code2);
+            return effects.attempt(referenceCollapsedConstruct, labelEndOk, labelEndNok)(code2);
         }
 
         function labelEndOk(code2) {
             return ok2(code2);
         }
 
         function labelEndNok(code2) {
@@ -22742,45 +25500,28 @@
             return markdownLineEndingOrSpace(code2) ? factoryWhitespace(effects, resourceOpen)(code2) : resourceOpen(code2);
         }
 
         function resourceOpen(code2) {
             if (code2 === 41) {
                 return resourceEnd(code2);
             }
-            return factoryDestination(
-                effects,
-                resourceDestinationAfter,
-                resourceDestinationMissing,
-                "resourceDestination",
-                "resourceDestinationLiteral",
-                "resourceDestinationLiteralMarker",
-                "resourceDestinationRaw",
-                "resourceDestinationString",
-                32
-            )(code2);
+            return factoryDestination(effects, resourceDestinationAfter, resourceDestinationMissing, "resourceDestination", "resourceDestinationLiteral", "resourceDestinationLiteralMarker", "resourceDestinationRaw", "resourceDestinationString", 32)(code2);
         }
 
         function resourceDestinationAfter(code2) {
             return markdownLineEndingOrSpace(code2) ? factoryWhitespace(effects, resourceBetween)(code2) : resourceEnd(code2);
         }
 
         function resourceDestinationMissing(code2) {
             return nok(code2);
         }
 
         function resourceBetween(code2) {
             if (code2 === 34 || code2 === 39 || code2 === 40) {
-                return factoryTitle(
-                    effects,
-                    resourceTitleAfter,
-                    nok,
-                    "resourceTitle",
-                    "resourceTitleMarker",
-                    "resourceTitleString"
-                )(code2);
+                return factoryTitle(effects, resourceTitleAfter, nok, "resourceTitle", "resourceTitleMarker", "resourceTitleString")(code2);
             }
             return resourceEnd(code2);
         }
 
         function resourceTitleAfter(code2) {
             return markdownLineEndingOrSpace(code2) ? factoryWhitespace(effects, resourceEnd)(code2) : resourceEnd(code2);
         }
@@ -22798,31 +25539,19 @@
     }
 
     function tokenizeReferenceFull(effects, ok2, nok) {
         const self2 = this;
         return referenceFull;
 
         function referenceFull(code2) {
-            return factoryLabel.call(
-                self2,
-                effects,
-                referenceFullAfter,
-                referenceFullMissing,
-                "reference",
-                "referenceMarker",
-                "referenceString"
-            )(code2);
+            return factoryLabel.call(self2, effects, referenceFullAfter, referenceFullMissing, "reference", "referenceMarker", "referenceString")(code2);
         }
 
         function referenceFullAfter(code2) {
-            return self2.parser.defined.includes(
-                normalizeIdentifier(
-                    self2.sliceSerialize(self2.events[self2.events.length - 1][1]).slice(1, -1)
-                )
-            ) ? ok2(code2) : nok(code2);
+            return self2.parser.defined.includes(normalizeIdentifier(self2.sliceSerialize(self2.events[self2.events.length - 1][1]).slice(1, -1))) ? ok2(code2) : nok(code2);
         }
 
         function referenceFullMissing(code2) {
             return nok(code2);
         }
     }
 
@@ -23023,19 +25752,15 @@
             effects.enter("listItemMarker");
             effects.consume(code2);
             effects.exit("listItemMarker");
             self2.containerState.marker = self2.containerState.marker || code2;
             return effects.check(
                 blankLine,
                 self2.interrupt ? nok : onBlank,
-                effects.attempt(
-                    listItemPrefixWhitespaceConstruct,
-                    endOfPrefix,
-                    otherPrefix
-                )
+                effects.attempt(listItemPrefixWhitespaceConstruct, endOfPrefix, otherPrefix)
             );
         }
 
         function onBlank(code2) {
             self2.containerState.initialBlankLine = true;
             initialSize++;
             return endOfPrefix(code2);
@@ -23060,20 +25785,15 @@
     function tokenizeListContinuation(effects, ok2, nok) {
         const self2 = this;
         self2.containerState._closeFlow = void 0;
         return effects.check(blankLine, onBlank, notBlank);
 
         function onBlank(code2) {
             self2.containerState.furtherBlankLines = self2.containerState.furtherBlankLines || self2.containerState.initialBlankLine;
-            return factorySpace(
-                effects,
-                ok2,
-                "listItemIndent",
-                self2.containerState.size + 1
-            )(code2);
+            return factorySpace(effects, ok2, "listItemIndent", self2.containerState.size + 1)(code2);
         }
 
         function notBlank(code2) {
             if (self2.containerState.furtherBlankLines || !markdownSpace(code2)) {
                 self2.containerState.furtherBlankLines = void 0;
                 self2.containerState.initialBlankLine = void 0;
                 return notInCurrentItem(code2);
@@ -23082,50 +25802,35 @@
             self2.containerState.initialBlankLine = void 0;
             return effects.attempt(indentConstruct, ok2, notInCurrentItem)(code2);
         }
 
         function notInCurrentItem(code2) {
             self2.containerState._closeFlow = true;
             self2.interrupt = void 0;
-            return factorySpace(
-                effects,
-                effects.attempt(list$2, ok2, nok),
-                "linePrefix",
-                self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4
-            )(code2);
+            return factorySpace(effects, effects.attempt(list$2, ok2, nok), "linePrefix", self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4)(code2);
         }
     }
 
     function tokenizeIndent$1(effects, ok2, nok) {
         const self2 = this;
-        return factorySpace(
-            effects,
-            afterPrefix,
-            "listItemIndent",
-            self2.containerState.size + 1
-        );
+        return factorySpace(effects, afterPrefix, "listItemIndent", self2.containerState.size + 1);
 
         function afterPrefix(code2) {
             const tail = self2.events[self2.events.length - 1];
             return tail && tail[1].type === "listItemIndent" && tail[2].sliceSerialize(tail[1], true).length === self2.containerState.size ? ok2(code2) : nok(code2);
         }
     }
 
     function tokenizeListEnd(effects) {
         effects.exit(this.containerState.type);
     }
 
     function tokenizeListItemPrefixWhitespace(effects, ok2, nok) {
         const self2 = this;
-        return factorySpace(
-            effects,
-            afterPrefix,
-            "listItemPrefixWhitespace",
-            self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4 + 1
-        );
+        return factorySpace(effects, afterPrefix, "listItemPrefixWhitespace", self2.parser.constructs.disable.null.includes("codeIndented") ? void 0 : 4 + 1);
 
         function afterPrefix(code2) {
             const tail = self2.events[self2.events.length - 1];
             return !markdownSpace(code2) && tail && tail[1].type === "listItemPrefixWhitespace" ? ok2(code2) : nok(code2);
         }
     }
     const setextUnderline = {
@@ -23950,15 +26655,15 @@
         if (head === 35) {
             const head2 = $2.charCodeAt(1);
             const hex2 = head2 === 120 || head2 === 88;
             return decodeNumericCharacterReference($2.slice(hex2 ? 2 : 1), hex2 ? 16 : 10);
         }
         return decodeNamedCharacterReference($2) || $0;
     }
-    const own$6 = {}.hasOwnProperty;
+    const own$7 = {}.hasOwnProperty;
 
     function fromMarkdown(value, encoding, options) {
         if (typeof encoding !== "string") {
             options = encoding;
             encoding = void 0;
         }
         return compiler(options)(
@@ -24096,15 +26801,15 @@
                         index2 = prepareList(events2, tail, index2);
                     }
                 }
             }
             index2 = -1;
             while (++index2 < events2.length) {
                 const handler = config2[events2[index2][0]];
-                if (own$6.call(handler, events2[index2][1].type)) {
+                if (own$7.call(handler, events2[index2][1].type)) {
                     handler[events2[index2][1].type].call(
                         Object.assign({
                                 sliceSerialize: events2[index2][2].sliceSerialize
                             },
                             context2
                         ),
                         events2[index2][1]
@@ -24699,15 +27404,15 @@
             }
         }
     }
 
     function extension$1(combined, extension2) {
         let key;
         for (key in extension2) {
-            if (own$6.call(extension2, key)) {
+            if (own$7.call(extension2, key)) {
                 switch (key) {
                     case "canContainEols": {
                         const right2 = extension2[key];
                         if (right2) {
                             combined[key].push(...right2);
                         }
                         break;
@@ -24894,15 +27599,15 @@
             properties: {},
             children: state.all(node2)
         };
         state.patch(node2, result);
         return state.applyData(node2, result);
     }
 
-    function html$2(state, node2) {
+    function html$4(state, node2) {
         if (state.options.allowDangerousHtml) {
             const result = {
                 type: "raw",
                 value: node2.value
             };
             state.patch(node2, result);
             return state.applyData(node2, result);
@@ -25338,15 +28043,15 @@
         blockquote: blockquote$1,
         break: hardBreak$1,
         code: code$3,
         delete: strikethrough,
         emphasis: emphasis$1,
         footnoteReference: footnoteReference$1,
         heading: heading$2,
-        html: html$2,
+        html: html$4,
         imageReference: imageReference$1,
         image: image$1,
         inlineCode: inlineCode$1,
         linkReference: linkReference$1,
         link: link$2,
         listItem: listItem$1,
         list: list$1,
@@ -25883,15 +28588,15 @@
 
         function overload(node2, parents) {
             const parent = parents[parents.length - 1];
             const index2 = parent ? parent.children.indexOf(node2) : void 0;
             return visitor(node2, index2, parent);
         }
     }
-    const own$5 = {}.hasOwnProperty;
+    const own$6 = {}.hasOwnProperty;
     const emptyOptions$1 = {};
 
     function createState(tree, options) {
         const settings2 = options || emptyOptions$1;
         const definitionById = /* @__PURE__ */ new Map();
         const footnoteById = /* @__PURE__ */ new Map();
         const footnoteCounts = /* @__PURE__ */ new Map();
@@ -25922,15 +28627,15 @@
             }
         });
         return state;
 
         function one2(node2, parent) {
             const type2 = node2.type;
             const handle2 = state.handlers[type2];
-            if (own$5.call(state.handlers, type2) && handle2) {
+            if (own$6.call(state.handlers, type2) && handle2) {
                 return handle2(state, node2, parent);
             }
             if (state.options.passThrough && state.options.passThrough.includes(type2)) {
                 if ("children" in node2) {
                     const {
                         children: children2,
                         ...shallow
@@ -26008,15 +28713,15 @@
             }
         }
         return result;
     }
 
     function defaultUnknownHandler(state, node2) {
         const data2 = node2.data || {};
-        const result = "value" in node2 && !(own$5.call(data2, "hProperties") || own$5.call(data2, "hChildren")) ? {
+        const result = "value" in node2 && !(own$6.call(data2, "hProperties") || own$6.call(data2, "hChildren")) ? {
             type: "text",
             value: node2.value
         } : {
             type: "element",
             tagName: "div",
             properties: {},
             children: state.all(node2)
@@ -26110,15 +28815,15 @@
     var gOPD$1 = Object.getOwnPropertyDescriptor;
     var isArray$9 = function isArray2(arr) {
         if (typeof Array.isArray === "function") {
             return Array.isArray(arr);
         }
         return toStr$2.call(arr) === "[object Array]";
     };
-    var isPlainObject$4 = function isPlainObject2(obj) {
+    var isPlainObject$5 = function isPlainObject2(obj) {
         if (!obj || toStr$2.call(obj) !== "[object Object]") {
             return false;
         }
         var hasOwnConstructor = hasOwn$2.call(obj, "constructor");
         var hasIsPrototypeOf = obj.constructor && obj.constructor.prototype && hasOwn$2.call(obj.constructor.prototype, "isPrototypeOf");
         if (obj.constructor && !hasOwnConstructor && !hasIsPrototypeOf) {
             return false;
@@ -26166,20 +28871,20 @@
         for (; i2 < length; ++i2) {
             options = arguments[i2];
             if (options != null) {
                 for (name2 in options) {
                     src = getProperty(target, name2);
                     copy2 = getProperty(options, name2);
                     if (target !== copy2) {
-                        if (deep && copy2 && (isPlainObject$4(copy2) || (copyIsArray = isArray$9(copy2)))) {
+                        if (deep && copy2 && (isPlainObject$5(copy2) || (copyIsArray = isArray$9(copy2)))) {
                             if (copyIsArray) {
                                 copyIsArray = false;
                                 clone2 = src && isArray$9(src) ? src : [];
                             } else {
-                                clone2 = src && isPlainObject$4(src) ? src : {};
+                                clone2 = src && isPlainObject$5(src) ? src : {};
                             }
                             setProperty(target, {
                                 name: name2,
                                 newValue: extend2(deep, clone2, copy2)
                             });
                         } else if (typeof copy2 !== "undefined") {
                             setProperty(target, {
@@ -26190,15 +28895,15 @@
                     }
                 }
             }
         }
         return target;
     };
 
-    function isPlainObject$3(value) {
+    function isPlainObject$4(value) {
         if (typeof value !== "object" || value === null) {
             return false;
         }
         const prototype = Object.getPrototypeOf(value);
         return (prototype === null || prototype === Object.prototype || Object.getPrototypeOf(prototype) === null) && !(Symbol.toStringTag in value) && !(Symbol.iterator in value);
     }
 
@@ -26266,15 +28971,15 @@
                 const exception = error2;
                 if (fnExpectsCallback && called) {
                     throw exception;
                 }
                 return done(exception);
             }
             if (!fnExpectsCallback) {
-                if (result instanceof Promise) {
+                if (result && result.then && typeof result.then === "function") {
                     result.then(then, done);
                 } else if (result instanceof Error) {
                     done(result);
                 } else {
                     then(result);
                 }
             }
@@ -26421,18 +29126,18 @@
         let joined;
         while (++index2 < segments.length) {
             assertPath$2(segments[index2]);
             if (segments[index2]) {
                 joined = joined === void 0 ? segments[index2] : joined + "/" + segments[index2];
             }
         }
-        return joined === void 0 ? "." : normalize$1(joined);
+        return joined === void 0 ? "." : normalize$2(joined);
     }
 
-    function normalize$1(path2) {
+    function normalize$2(path2) {
         assertPath$2(path2);
         const absolute = path2.codePointAt(0) === 47;
         let value = normalizeString(path2, !absolute);
         if (value.length === 0 && !absolute) {
             value = ".";
         }
         if (value.length > 0 && path2.codePointAt(path2.length - 1) === 47) {
@@ -26566,15 +29271,15 @@
                     error2.code = "ERR_INVALID_FILE_URL_PATH";
                     throw error2;
                 }
             }
         }
         return decodeURIComponent(pathname);
     }
-    const order$2 = [
+    const order$1 = [
         "history",
         "path",
         "basename",
         "stem",
         "extname",
         "dirname"
     ];
@@ -26599,23 +29304,23 @@
             this.history = [];
             this.messages = [];
             this.value;
             this.map;
             this.result;
             this.stored;
             let index2 = -1;
-            while (++index2 < order$2.length) {
-                const prop2 = order$2[index2];
+            while (++index2 < order$1.length) {
+                const prop2 = order$1[index2];
                 if (prop2 in options && options[prop2] !== void 0 && options[prop2] !== null) {
                     this[prop2] = prop2 === "history" ? [...options[prop2]] : options[prop2];
                 }
             }
             let prop;
             for (prop in options) {
-                if (!order$2.includes(prop)) {
+                if (!order$1.includes(prop)) {
                     this[prop] = options[prop];
                 }
             }
         }
         get basename() {
             return typeof this.path === "string" ? path$2.basename(this.path) : void 0;
         }
@@ -26741,15 +29446,15 @@
         for (const p2 of names) {
             const descriptor = Object.getOwnPropertyDescriptor(func, p2);
             if (descriptor)
                 Object.defineProperty(apply, p2, descriptor);
         }
         return apply;
     };
-    const own$4 = {}.hasOwnProperty;
+    const own$5 = {}.hasOwnProperty;
     class Processor extends CallableInstance {
         constructor() {
             super("copy");
             this.Compiler = void 0;
             this.Parser = void 0;
             this.attachers = [];
             this.compiler = void 0;
@@ -26772,15 +29477,15 @@
         data(key, value) {
             if (typeof key === "string") {
                 if (arguments.length === 2) {
                     assertUnfrozen("data", this.frozen);
                     this.namespace[key] = value;
                     return this;
                 }
-                return own$4.call(this.namespace, key) && this.namespace[key] || void 0;
+                return own$5.call(this.namespace, key) && this.namespace[key] || void 0;
             }
             if (key) {
                 assertUnfrozen("data", this.frozen);
                 this.namespace = key;
                 return this;
             }
             return this.namespace;
@@ -26982,15 +29687,15 @@
                     }
                 }
                 if (entryIndex === -1) {
                     attachers.push([plugin, ...parameters2]);
                 } else if (parameters2.length > 0) {
                     let [primary, ...rest] = parameters2;
                     const currentPrimary = attachers[entryIndex][1];
-                    if (isPlainObject$3(currentPrimary) && isPlainObject$3(primary)) {
+                    if (isPlainObject$4(currentPrimary) && isPlainObject$4(primary)) {
                         primary = extend$3(true, currentPrimary, primary);
                     }
                     attachers[entryIndex] = [plugin, primary, ...rest];
                 }
             }
         }
     }
@@ -27013,15 +29718,15 @@
             throw new Error(
                 "Cannot call `" + name2 + "` on a frozen processor.\nCreate a new processor first, by calling it: use `processor()` instead of `processor`."
             );
         }
     }
 
     function assertNode(node2) {
-        if (!isPlainObject$3(node2) || typeof node2.type !== "string") {
+        if (!isPlainObject$4(node2) || typeof node2.type !== "string") {
             throw new TypeError("Expected node, got `" + node2 + "`");
         }
     }
 
     function assertDone(name2, asyncName, complete) {
         if (!complete) {
             throw new Error(
@@ -27858,25 +30563,25 @@
         return value.length;
     }
 
     function toAlignment(value) {
         const code2 = typeof value === "string" ? value.codePointAt(0) : 0;
         return code2 === 67 || code2 === 99 ? 99 : code2 === 76 || code2 === 108 ? 108 : code2 === 82 || code2 === 114 ? 114 : 0;
     }
-    const own$3 = {}.hasOwnProperty;
+    const own$4 = {}.hasOwnProperty;
 
     function zwitch(key, options) {
         const settings2 = options || {};
 
         function one2(value, ...parameters) {
             let fn2 = one2.invalid;
             const handlers2 = one2.handlers;
-            if (value && own$3.call(value, key)) {
+            if (value && own$4.call(value, key)) {
                 const id2 = String(value[key]);
-                fn2 = own$3.call(handlers2, id2) ? handlers2[id2] : one2.unknown;
+                fn2 = own$4.call(handlers2, id2) ? handlers2[id2] : one2.unknown;
             }
             if (fn2) {
                 return fn2.call(this, value, ...parameters);
             }
         }
         one2.handlers = settings2.handlers || {};
         one2.invalid = settings2.invalid;
@@ -28165,17 +30870,17 @@
         if (state.options.closeAtx) {
             value += " " + sequence;
         }
         subexit();
         exit2();
         return value;
     }
-    html$1.peek = htmlPeek;
+    html$3.peek = htmlPeek;
 
-    function html$1(node2) {
+    function html$3(node2) {
         return node2.value || "";
     }
 
     function htmlPeek() {
         return "<";
     }
     image.peek = imagePeek;
@@ -28647,15 +31352,15 @@
         blockquote,
         break: hardBreak,
         code: code$2,
         definition,
         emphasis,
         hardBreak,
         heading: heading$1,
-        html: html$1,
+        html: html$3,
         image,
         imageReference,
         inlineCode,
         link: link$1,
         linkReference,
         list,
         listItem,
@@ -30622,98 +33327,98 @@
             style: style2,
             children: jsxRuntime.exports.jsx(Markdown$2, Object.assign({}, reactMarkdownProps, {
                 remarkPlugins: (_a3 = reactMarkdownProps.remarkPlugins) !== null && _a3 !== void 0 ? _a3 : [remarkGfm],
                 children: markdown
             }))
         });
     }
-    var top$2 = "top";
-    var bottom$1 = "bottom";
-    var right$1 = "right";
-    var left$1 = "left";
-    var auto$1 = "auto";
-    var basePlacements$1 = [top$2, bottom$1, right$1, left$1];
-    var start$2 = "start";
-    var end$1 = "end";
-    var clippingParents$1 = "clippingParents";
-    var viewport$1 = "viewport";
-    var popper$1 = "popper";
-    var reference$1 = "reference";
-    var variationPlacements$1 = /* @__PURE__ */ basePlacements$1.reduce(function(acc, placement) {
-        return acc.concat([placement + "-" + start$2, placement + "-" + end$1]);
+    var top$1 = "top";
+    var bottom = "bottom";
+    var right = "right";
+    var left = "left";
+    var auto = "auto";
+    var basePlacements = [top$1, bottom, right, left];
+    var start$1 = "start";
+    var end = "end";
+    var clippingParents = "clippingParents";
+    var viewport = "viewport";
+    var popper = "popper";
+    var reference = "reference";
+    var variationPlacements = /* @__PURE__ */ basePlacements.reduce(function(acc, placement) {
+        return acc.concat([placement + "-" + start$1, placement + "-" + end]);
     }, []);
-    var placements$2 = /* @__PURE__ */ [].concat(basePlacements$1, [auto$1]).reduce(function(acc, placement) {
-        return acc.concat([placement, placement + "-" + start$2, placement + "-" + end$1]);
+    var placements = /* @__PURE__ */ [].concat(basePlacements, [auto]).reduce(function(acc, placement) {
+        return acc.concat([placement, placement + "-" + start$1, placement + "-" + end]);
     }, []);
-    var beforeRead$1 = "beforeRead";
-    var read$1 = "read";
-    var afterRead$1 = "afterRead";
-    var beforeMain$1 = "beforeMain";
-    var main$1 = "main";
-    var afterMain$1 = "afterMain";
-    var beforeWrite$1 = "beforeWrite";
-    var write$1 = "write";
-    var afterWrite$1 = "afterWrite";
-    var modifierPhases$1 = [beforeRead$1, read$1, afterRead$1, beforeMain$1, main$1, afterMain$1, beforeWrite$1, write$1, afterWrite$1];
+    var beforeRead = "beforeRead";
+    var read = "read";
+    var afterRead = "afterRead";
+    var beforeMain = "beforeMain";
+    var main = "main";
+    var afterMain = "afterMain";
+    var beforeWrite = "beforeWrite";
+    var write = "write";
+    var afterWrite = "afterWrite";
+    var modifierPhases = [beforeRead, read, afterRead, beforeMain, main, afterMain, beforeWrite, write, afterWrite];
 
-    function getNodeName$2(element2) {
+    function getNodeName(element2) {
         return element2 ? (element2.nodeName || "").toLowerCase() : null;
     }
 
-    function getWindow$2(node2) {
+    function getWindow(node2) {
         if (node2 == null) {
             return window;
         }
         if (node2.toString() !== "[object Window]") {
             var ownerDocument = node2.ownerDocument;
             return ownerDocument ? ownerDocument.defaultView || window : window;
         }
         return node2;
     }
 
-    function isElement$5(node2) {
-        var OwnElement = getWindow$2(node2).Element;
+    function isElement$3(node2) {
+        var OwnElement = getWindow(node2).Element;
         return node2 instanceof OwnElement || node2 instanceof Element;
     }
 
-    function isHTMLElement$2(node2) {
-        var OwnElement = getWindow$2(node2).HTMLElement;
+    function isHTMLElement(node2) {
+        var OwnElement = getWindow(node2).HTMLElement;
         return node2 instanceof OwnElement || node2 instanceof HTMLElement;
     }
 
-    function isShadowRoot$1(node2) {
+    function isShadowRoot(node2) {
         if (typeof ShadowRoot === "undefined") {
             return false;
         }
-        var OwnElement = getWindow$2(node2).ShadowRoot;
+        var OwnElement = getWindow(node2).ShadowRoot;
         return node2 instanceof OwnElement || node2 instanceof ShadowRoot;
     }
 
-    function applyStyles$2(_ref2) {
+    function applyStyles(_ref2) {
         var state = _ref2.state;
         Object.keys(state.elements).forEach(function(name2) {
             var style2 = state.styles[name2] || {};
             var attributes2 = state.attributes[name2] || {};
             var element2 = state.elements[name2];
-            if (!isHTMLElement$2(element2) || !getNodeName$2(element2)) {
+            if (!isHTMLElement(element2) || !getNodeName(element2)) {
                 return;
             }
             Object.assign(element2.style, style2);
             Object.keys(attributes2).forEach(function(name3) {
                 var value = attributes2[name3];
                 if (value === false) {
                     element2.removeAttribute(name3);
                 } else {
                     element2.setAttribute(name3, value === true ? "" : value);
                 }
             });
         });
     }
 
-    function effect$5(_ref2) {
+    function effect$2(_ref2) {
         var state = _ref2.state;
         var initialStyles = {
             popper: {
                 position: state.options.strategy,
                 left: "0",
                 top: "0",
                 margin: "0"
@@ -30733,39 +33438,39 @@
                 var element2 = state.elements[name2];
                 var attributes2 = state.attributes[name2] || {};
                 var styleProperties = Object.keys(state.styles.hasOwnProperty(name2) ? state.styles[name2] : initialStyles[name2]);
                 var style2 = styleProperties.reduce(function(style3, property) {
                     style3[property] = "";
                     return style3;
                 }, {});
-                if (!isHTMLElement$2(element2) || !getNodeName$2(element2)) {
+                if (!isHTMLElement(element2) || !getNodeName(element2)) {
                     return;
                 }
                 Object.assign(element2.style, style2);
                 Object.keys(attributes2).forEach(function(attribute) {
                     element2.removeAttribute(attribute);
                 });
             });
         };
     }
-    const applyStyles$3 = {
+    const applyStyles$1 = {
         name: "applyStyles",
         enabled: true,
         phase: "write",
-        fn: applyStyles$2,
-        effect: effect$5,
+        fn: applyStyles,
+        effect: effect$2,
         requires: ["computeStyles"]
     };
 
-    function getBasePlacement$3(placement) {
+    function getBasePlacement$2(placement) {
         return placement.split("-")[0];
     }
-    var max$4 = Math.max;
-    var min$3 = Math.min;
-    var round$3 = Math.round;
+    var max$3 = Math.max;
+    var min$2 = Math.min;
+    var round$2 = Math.round;
 
     function getUAString() {
         var uaData = navigator.userAgentData;
         if (uaData != null && uaData.brands && Array.isArray(uaData.brands)) {
             return uaData.brands.map(function(item) {
                 return item.brand + "/" + item.version;
             }).join(" ");
@@ -30773,29 +33478,29 @@
         return navigator.userAgent;
     }
 
     function isLayoutViewport() {
         return !/^((?!chrome|android).)*safari/i.test(getUAString());
     }
 
-    function getBoundingClientRect$2(element2, includeScale, isFixedStrategy) {
+    function getBoundingClientRect(element2, includeScale, isFixedStrategy) {
         if (includeScale === void 0) {
             includeScale = false;
         }
         if (isFixedStrategy === void 0) {
             isFixedStrategy = false;
         }
         var clientRect = element2.getBoundingClientRect();
         var scaleX = 1;
         var scaleY = 1;
-        if (includeScale && isHTMLElement$2(element2)) {
-            scaleX = element2.offsetWidth > 0 ? round$3(clientRect.width) / element2.offsetWidth || 1 : 1;
-            scaleY = element2.offsetHeight > 0 ? round$3(clientRect.height) / element2.offsetHeight || 1 : 1;
+        if (includeScale && isHTMLElement(element2)) {
+            scaleX = element2.offsetWidth > 0 ? round$2(clientRect.width) / element2.offsetWidth || 1 : 1;
+            scaleY = element2.offsetHeight > 0 ? round$2(clientRect.height) / element2.offsetHeight || 1 : 1;
         }
-        var _ref2 = isElement$5(element2) ? getWindow$2(element2) : window,
+        var _ref2 = isElement$3(element2) ? getWindow(element2) : window,
             visualViewport = _ref2.visualViewport;
         var addVisualOffsets = !isLayoutViewport() && isFixedStrategy;
         var x2 = (clientRect.left + (addVisualOffsets && visualViewport ? visualViewport.offsetLeft : 0)) / scaleX;
         var y2 = (clientRect.top + (addVisualOffsets && visualViewport ? visualViewport.offsetTop : 0)) / scaleY;
         var width = clientRect.width / scaleX;
         var height = clientRect.height / scaleY;
         return {
@@ -30806,16 +33511,16 @@
             bottom: y2 + height,
             left: x2,
             x: x2,
             y: y2
         };
     }
 
-    function getLayoutRect$1(element2) {
-        var clientRect = getBoundingClientRect$2(element2);
+    function getLayoutRect(element2) {
+        var clientRect = getBoundingClientRect(element2);
         var width = element2.offsetWidth;
         var height = element2.offsetHeight;
         if (Math.abs(clientRect.width - width) <= 1) {
             width = clientRect.width;
         }
         if (Math.abs(clientRect.height - height) <= 1) {
             height = clientRect.height;
@@ -30824,410 +33529,410 @@
             x: element2.offsetLeft,
             y: element2.offsetTop,
             width,
             height
         };
     }
 
-    function contains$2(parent, child) {
+    function contains$1(parent, child) {
         var rootNode = child.getRootNode && child.getRootNode();
         if (parent.contains(child)) {
             return true;
-        } else if (rootNode && isShadowRoot$1(rootNode)) {
+        } else if (rootNode && isShadowRoot(rootNode)) {
             var next2 = child;
             do {
                 if (next2 && parent.isSameNode(next2)) {
                     return true;
                 }
                 next2 = next2.parentNode || next2.host;
             } while (next2);
         }
         return false;
     }
 
-    function getComputedStyle$3(element2) {
-        return getWindow$2(element2).getComputedStyle(element2);
+    function getComputedStyle$1(element2) {
+        return getWindow(element2).getComputedStyle(element2);
     }
 
-    function isTableElement$2(element2) {
-        return ["table", "td", "th"].indexOf(getNodeName$2(element2)) >= 0;
+    function isTableElement(element2) {
+        return ["table", "td", "th"].indexOf(getNodeName(element2)) >= 0;
     }
 
-    function getDocumentElement$2(element2) {
-        return ((isElement$5(element2) ? element2.ownerDocument : element2.document) || window.document).documentElement;
+    function getDocumentElement(element2) {
+        return ((isElement$3(element2) ? element2.ownerDocument : element2.document) || window.document).documentElement;
     }
 
-    function getParentNode$2(element2) {
-        if (getNodeName$2(element2) === "html") {
+    function getParentNode(element2) {
+        if (getNodeName(element2) === "html") {
             return element2;
         }
-        return element2.assignedSlot || element2.parentNode || (isShadowRoot$1(element2) ? element2.host : null) || getDocumentElement$2(element2);
+        return element2.assignedSlot || element2.parentNode || (isShadowRoot(element2) ? element2.host : null) || getDocumentElement(element2);
     }
 
-    function getTrueOffsetParent$2(element2) {
-        if (!isHTMLElement$2(element2) || getComputedStyle$3(element2).position === "fixed") {
+    function getTrueOffsetParent(element2) {
+        if (!isHTMLElement(element2) || getComputedStyle$1(element2).position === "fixed") {
             return null;
         }
         return element2.offsetParent;
     }
 
-    function getContainingBlock$1(element2) {
+    function getContainingBlock(element2) {
         var isFirefox2 = /firefox/i.test(getUAString());
         var isIE2 = /Trident/i.test(getUAString());
-        if (isIE2 && isHTMLElement$2(element2)) {
-            var elementCss = getComputedStyle$3(element2);
+        if (isIE2 && isHTMLElement(element2)) {
+            var elementCss = getComputedStyle$1(element2);
             if (elementCss.position === "fixed") {
                 return null;
             }
         }
-        var currentNode = getParentNode$2(element2);
-        if (isShadowRoot$1(currentNode)) {
+        var currentNode = getParentNode(element2);
+        if (isShadowRoot(currentNode)) {
             currentNode = currentNode.host;
         }
-        while (isHTMLElement$2(currentNode) && ["html", "body"].indexOf(getNodeName$2(currentNode)) < 0) {
-            var css2 = getComputedStyle$3(currentNode);
+        while (isHTMLElement(currentNode) && ["html", "body"].indexOf(getNodeName(currentNode)) < 0) {
+            var css2 = getComputedStyle$1(currentNode);
             if (css2.transform !== "none" || css2.perspective !== "none" || css2.contain === "paint" || ["transform", "perspective"].indexOf(css2.willChange) !== -1 || isFirefox2 && css2.willChange === "filter" || isFirefox2 && css2.filter && css2.filter !== "none") {
                 return currentNode;
             } else {
                 currentNode = currentNode.parentNode;
             }
         }
         return null;
     }
 
-    function getOffsetParent$2(element2) {
-        var window2 = getWindow$2(element2);
-        var offsetParent = getTrueOffsetParent$2(element2);
-        while (offsetParent && isTableElement$2(offsetParent) && getComputedStyle$3(offsetParent).position === "static") {
-            offsetParent = getTrueOffsetParent$2(offsetParent);
+    function getOffsetParent(element2) {
+        var window2 = getWindow(element2);
+        var offsetParent = getTrueOffsetParent(element2);
+        while (offsetParent && isTableElement(offsetParent) && getComputedStyle$1(offsetParent).position === "static") {
+            offsetParent = getTrueOffsetParent(offsetParent);
         }
-        if (offsetParent && (getNodeName$2(offsetParent) === "html" || getNodeName$2(offsetParent) === "body" && getComputedStyle$3(offsetParent).position === "static")) {
+        if (offsetParent && (getNodeName(offsetParent) === "html" || getNodeName(offsetParent) === "body" && getComputedStyle$1(offsetParent).position === "static")) {
             return window2;
         }
-        return offsetParent || getContainingBlock$1(element2) || window2;
+        return offsetParent || getContainingBlock(element2) || window2;
     }
 
-    function getMainAxisFromPlacement$1(placement) {
+    function getMainAxisFromPlacement(placement) {
         return ["top", "bottom"].indexOf(placement) >= 0 ? "x" : "y";
     }
 
-    function within$1(min2, value, max2) {
-        return max$4(min2, min$3(value, max2));
+    function within(min2, value, max2) {
+        return max$3(min2, min$2(value, max2));
     }
 
     function withinMaxClamp(min2, value, max2) {
-        var v3 = within$1(min2, value, max2);
+        var v3 = within(min2, value, max2);
         return v3 > max2 ? max2 : v3;
     }
 
-    function getFreshSideObject$1() {
+    function getFreshSideObject() {
         return {
             top: 0,
             right: 0,
             bottom: 0,
             left: 0
         };
     }
 
-    function mergePaddingObject$1(paddingObject) {
-        return Object.assign({}, getFreshSideObject$1(), paddingObject);
+    function mergePaddingObject(paddingObject) {
+        return Object.assign({}, getFreshSideObject(), paddingObject);
     }
 
-    function expandToHashMap$1(value, keys2) {
+    function expandToHashMap(value, keys2) {
         return keys2.reduce(function(hashMap, key) {
             hashMap[key] = value;
             return hashMap;
         }, {});
     }
     var toPaddingObject = function toPaddingObject2(padding, state) {
         padding = typeof padding === "function" ? padding(Object.assign({}, state.rects, {
             placement: state.placement
         })) : padding;
-        return mergePaddingObject$1(typeof padding !== "number" ? padding : expandToHashMap$1(padding, basePlacements$1));
+        return mergePaddingObject(typeof padding !== "number" ? padding : expandToHashMap(padding, basePlacements));
     };
 
-    function arrow$3(_ref2) {
+    function arrow(_ref2) {
         var _state$modifiersData$;
         var state = _ref2.state,
             name2 = _ref2.name,
             options = _ref2.options;
         var arrowElement = state.elements.arrow;
         var popperOffsets2 = state.modifiersData.popperOffsets;
-        var basePlacement = getBasePlacement$3(state.placement);
-        var axis = getMainAxisFromPlacement$1(basePlacement);
-        var isVertical = [left$1, right$1].indexOf(basePlacement) >= 0;
+        var basePlacement = getBasePlacement$2(state.placement);
+        var axis = getMainAxisFromPlacement(basePlacement);
+        var isVertical = [left, right].indexOf(basePlacement) >= 0;
         var len = isVertical ? "height" : "width";
         if (!arrowElement || !popperOffsets2) {
             return;
         }
         var paddingObject = toPaddingObject(options.padding, state);
-        var arrowRect = getLayoutRect$1(arrowElement);
-        var minProp = axis === "y" ? top$2 : left$1;
-        var maxProp = axis === "y" ? bottom$1 : right$1;
+        var arrowRect = getLayoutRect(arrowElement);
+        var minProp = axis === "y" ? top$1 : left;
+        var maxProp = axis === "y" ? bottom : right;
         var endDiff = state.rects.reference[len] + state.rects.reference[axis] - popperOffsets2[axis] - state.rects.popper[len];
         var startDiff = popperOffsets2[axis] - state.rects.reference[axis];
-        var arrowOffsetParent = getOffsetParent$2(arrowElement);
+        var arrowOffsetParent = getOffsetParent(arrowElement);
         var clientSize = arrowOffsetParent ? axis === "y" ? arrowOffsetParent.clientHeight || 0 : arrowOffsetParent.clientWidth || 0 : 0;
         var centerToReference = endDiff / 2 - startDiff / 2;
         var min2 = paddingObject[minProp];
         var max2 = clientSize - arrowRect[len] - paddingObject[maxProp];
         var center2 = clientSize / 2 - arrowRect[len] / 2 + centerToReference;
-        var offset2 = within$1(min2, center2, max2);
+        var offset2 = within(min2, center2, max2);
         var axisProp = axis;
         state.modifiersData[name2] = (_state$modifiersData$ = {}, _state$modifiersData$[axisProp] = offset2, _state$modifiersData$.centerOffset = offset2 - center2, _state$modifiersData$);
     }
 
-    function effect$4(_ref2) {
+    function effect$1(_ref2) {
         var state = _ref2.state,
             options = _ref2.options;
         var _options$element = options.element,
             arrowElement = _options$element === void 0 ? "[data-popper-arrow]" : _options$element;
         if (arrowElement == null) {
             return;
         }
         if (typeof arrowElement === "string") {
             arrowElement = state.elements.popper.querySelector(arrowElement);
             if (!arrowElement) {
                 return;
             }
         }
-        if (!contains$2(state.elements.popper, arrowElement)) {
+        if (!contains$1(state.elements.popper, arrowElement)) {
             return;
         }
         state.elements.arrow = arrowElement;
     }
-    const arrow$4 = {
+    const arrow$1 = {
         name: "arrow",
         enabled: true,
         phase: "main",
-        fn: arrow$3,
-        effect: effect$4,
+        fn: arrow,
+        effect: effect$1,
         requires: ["popperOffsets"],
         requiresIfExists: ["preventOverflow"]
     };
 
-    function getVariation$1(placement) {
+    function getVariation(placement) {
         return placement.split("-")[1];
     }
-    var unsetSides$1 = {
+    var unsetSides = {
         top: "auto",
         right: "auto",
         bottom: "auto",
         left: "auto"
     };
 
     function roundOffsetsByDPR(_ref2, win) {
         var x2 = _ref2.x,
             y2 = _ref2.y;
         var dpr = win.devicePixelRatio || 1;
         return {
-            x: round$3(x2 * dpr) / dpr || 0,
-            y: round$3(y2 * dpr) / dpr || 0
+            x: round$2(x2 * dpr) / dpr || 0,
+            y: round$2(y2 * dpr) / dpr || 0
         };
     }
 
-    function mapToStyles$1(_ref2) {
+    function mapToStyles(_ref2) {
         var _Object$assign2;
         var popper2 = _ref2.popper,
             popperRect = _ref2.popperRect,
             placement = _ref2.placement,
             variation = _ref2.variation,
             offsets = _ref2.offsets,
             position2 = _ref2.position,
             gpuAcceleration = _ref2.gpuAcceleration,
             adaptive = _ref2.adaptive,
-            roundOffsets2 = _ref2.roundOffsets,
+            roundOffsets = _ref2.roundOffsets,
             isFixed = _ref2.isFixed;
         var _offsets$x = offsets.x,
             x2 = _offsets$x === void 0 ? 0 : _offsets$x,
             _offsets$y = offsets.y,
             y2 = _offsets$y === void 0 ? 0 : _offsets$y;
-        var _ref3 = typeof roundOffsets2 === "function" ? roundOffsets2({
+        var _ref3 = typeof roundOffsets === "function" ? roundOffsets({
             x: x2,
             y: y2
         }) : {
             x: x2,
             y: y2
         };
         x2 = _ref3.x;
         y2 = _ref3.y;
         var hasX = offsets.hasOwnProperty("x");
         var hasY = offsets.hasOwnProperty("y");
-        var sideX = left$1;
-        var sideY = top$2;
+        var sideX = left;
+        var sideY = top$1;
         var win = window;
         if (adaptive) {
-            var offsetParent = getOffsetParent$2(popper2);
+            var offsetParent = getOffsetParent(popper2);
             var heightProp = "clientHeight";
             var widthProp = "clientWidth";
-            if (offsetParent === getWindow$2(popper2)) {
-                offsetParent = getDocumentElement$2(popper2);
-                if (getComputedStyle$3(offsetParent).position !== "static" && position2 === "absolute") {
+            if (offsetParent === getWindow(popper2)) {
+                offsetParent = getDocumentElement(popper2);
+                if (getComputedStyle$1(offsetParent).position !== "static" && position2 === "absolute") {
                     heightProp = "scrollHeight";
                     widthProp = "scrollWidth";
                 }
             }
             offsetParent = offsetParent;
-            if (placement === top$2 || (placement === left$1 || placement === right$1) && variation === end$1) {
-                sideY = bottom$1;
+            if (placement === top$1 || (placement === left || placement === right) && variation === end) {
+                sideY = bottom;
                 var offsetY = isFixed && offsetParent === win && win.visualViewport ? win.visualViewport.height : offsetParent[heightProp];
                 y2 -= offsetY - popperRect.height;
                 y2 *= gpuAcceleration ? 1 : -1;
             }
-            if (placement === left$1 || (placement === top$2 || placement === bottom$1) && variation === end$1) {
-                sideX = right$1;
+            if (placement === left || (placement === top$1 || placement === bottom) && variation === end) {
+                sideX = right;
                 var offsetX = isFixed && offsetParent === win && win.visualViewport ? win.visualViewport.width : offsetParent[widthProp];
                 x2 -= offsetX - popperRect.width;
                 x2 *= gpuAcceleration ? 1 : -1;
             }
         }
         var commonStyles = Object.assign({
             position: position2
-        }, adaptive && unsetSides$1);
-        var _ref4 = roundOffsets2 === true ? roundOffsetsByDPR({
+        }, adaptive && unsetSides);
+        var _ref4 = roundOffsets === true ? roundOffsetsByDPR({
             x: x2,
             y: y2
-        }, getWindow$2(popper2)) : {
+        }, getWindow(popper2)) : {
             x: x2,
             y: y2
         };
         x2 = _ref4.x;
         y2 = _ref4.y;
         if (gpuAcceleration) {
             var _Object$assign;
             return Object.assign({}, commonStyles, (_Object$assign = {}, _Object$assign[sideY] = hasY ? "0" : "", _Object$assign[sideX] = hasX ? "0" : "", _Object$assign.transform = (win.devicePixelRatio || 1) <= 1 ? "translate(" + x2 + "px, " + y2 + "px)" : "translate3d(" + x2 + "px, " + y2 + "px, 0)", _Object$assign));
         }
         return Object.assign({}, commonStyles, (_Object$assign2 = {}, _Object$assign2[sideY] = hasY ? y2 + "px" : "", _Object$assign2[sideX] = hasX ? x2 + "px" : "", _Object$assign2.transform = "", _Object$assign2));
     }
 
-    function computeStyles$2(_ref5) {
+    function computeStyles(_ref5) {
         var state = _ref5.state,
             options = _ref5.options;
         var _options$gpuAccelerat = options.gpuAcceleration,
             gpuAcceleration = _options$gpuAccelerat === void 0 ? true : _options$gpuAccelerat,
             _options$adaptive = options.adaptive,
             adaptive = _options$adaptive === void 0 ? true : _options$adaptive,
             _options$roundOffsets = options.roundOffsets,
-            roundOffsets2 = _options$roundOffsets === void 0 ? true : _options$roundOffsets;
+            roundOffsets = _options$roundOffsets === void 0 ? true : _options$roundOffsets;
         var commonStyles = {
-            placement: getBasePlacement$3(state.placement),
-            variation: getVariation$1(state.placement),
+            placement: getBasePlacement$2(state.placement),
+            variation: getVariation(state.placement),
             popper: state.elements.popper,
             popperRect: state.rects.popper,
             gpuAcceleration,
             isFixed: state.options.strategy === "fixed"
         };
         if (state.modifiersData.popperOffsets != null) {
-            state.styles.popper = Object.assign({}, state.styles.popper, mapToStyles$1(Object.assign({}, commonStyles, {
+            state.styles.popper = Object.assign({}, state.styles.popper, mapToStyles(Object.assign({}, commonStyles, {
                 offsets: state.modifiersData.popperOffsets,
                 position: state.options.strategy,
                 adaptive,
-                roundOffsets: roundOffsets2
+                roundOffsets
             })));
         }
         if (state.modifiersData.arrow != null) {
-            state.styles.arrow = Object.assign({}, state.styles.arrow, mapToStyles$1(Object.assign({}, commonStyles, {
+            state.styles.arrow = Object.assign({}, state.styles.arrow, mapToStyles(Object.assign({}, commonStyles, {
                 offsets: state.modifiersData.arrow,
                 position: "absolute",
                 adaptive: false,
-                roundOffsets: roundOffsets2
+                roundOffsets
             })));
         }
         state.attributes.popper = Object.assign({}, state.attributes.popper, {
             "data-popper-placement": state.placement
         });
     }
-    const computeStyles$3 = {
+    const computeStyles$1 = {
         name: "computeStyles",
         enabled: true,
         phase: "beforeWrite",
-        fn: computeStyles$2,
+        fn: computeStyles,
         data: {}
     };
-    var passive$1 = {
+    var passive = {
         passive: true
     };
 
-    function effect$3(_ref2) {
+    function effect(_ref2) {
         var state = _ref2.state,
             instance2 = _ref2.instance,
             options = _ref2.options;
         var _options$scroll = options.scroll,
             scroll = _options$scroll === void 0 ? true : _options$scroll,
             _options$resize = options.resize,
             resize = _options$resize === void 0 ? true : _options$resize;
-        var window2 = getWindow$2(state.elements.popper);
+        var window2 = getWindow(state.elements.popper);
         var scrollParents = [].concat(state.scrollParents.reference, state.scrollParents.popper);
         if (scroll) {
             scrollParents.forEach(function(scrollParent) {
-                scrollParent.addEventListener("scroll", instance2.update, passive$1);
+                scrollParent.addEventListener("scroll", instance2.update, passive);
             });
         }
         if (resize) {
-            window2.addEventListener("resize", instance2.update, passive$1);
+            window2.addEventListener("resize", instance2.update, passive);
         }
         return function() {
             if (scroll) {
                 scrollParents.forEach(function(scrollParent) {
-                    scrollParent.removeEventListener("scroll", instance2.update, passive$1);
+                    scrollParent.removeEventListener("scroll", instance2.update, passive);
                 });
             }
             if (resize) {
-                window2.removeEventListener("resize", instance2.update, passive$1);
+                window2.removeEventListener("resize", instance2.update, passive);
             }
         };
     }
-    const eventListeners$1 = {
+    const eventListeners = {
         name: "eventListeners",
         enabled: true,
         phase: "write",
         fn: function fn2() {},
-        effect: effect$3,
+        effect,
         data: {}
     };
-    var hash$4 = {
+    var hash$2 = {
         left: "right",
         right: "left",
         bottom: "top",
         top: "bottom"
     };
 
-    function getOppositePlacement$2(placement) {
+    function getOppositePlacement(placement) {
         return placement.replace(/left|right|bottom|top/g, function(matched) {
-            return hash$4[matched];
+            return hash$2[matched];
         });
     }
-    var hash$3 = {
+    var hash$1 = {
         start: "end",
         end: "start"
     };
 
-    function getOppositeVariationPlacement$1(placement) {
+    function getOppositeVariationPlacement(placement) {
         return placement.replace(/start|end/g, function(matched) {
-            return hash$3[matched];
+            return hash$1[matched];
         });
     }
 
-    function getWindowScroll$1(node2) {
-        var win = getWindow$2(node2);
+    function getWindowScroll(node2) {
+        var win = getWindow(node2);
         var scrollLeft = win.pageXOffset;
         var scrollTop = win.pageYOffset;
         return {
             scrollLeft,
             scrollTop
         };
     }
 
-    function getWindowScrollBarX$2(element2) {
-        return getBoundingClientRect$2(getDocumentElement$2(element2)).left + getWindowScroll$1(element2).scrollLeft;
+    function getWindowScrollBarX(element2) {
+        return getBoundingClientRect(getDocumentElement(element2)).left + getWindowScroll(element2).scrollLeft;
     }
 
-    function getViewportRect$2(element2, strategy) {
-        var win = getWindow$2(element2);
-        var html2 = getDocumentElement$2(element2);
+    function getViewportRect(element2, strategy) {
+        var win = getWindow(element2);
+        var html2 = getDocumentElement(element2);
         var visualViewport = win.visualViewport;
         var width = html2.clientWidth;
         var height = html2.clientHeight;
         var x2 = 0;
         var y2 = 0;
         if (visualViewport) {
             width = visualViewport.width;
@@ -31237,278 +33942,278 @@
                 x2 = visualViewport.offsetLeft;
                 y2 = visualViewport.offsetTop;
             }
         }
         return {
             width,
             height,
-            x: x2 + getWindowScrollBarX$2(element2),
+            x: x2 + getWindowScrollBarX(element2),
             y: y2
         };
     }
 
-    function getDocumentRect$2(element2) {
+    function getDocumentRect(element2) {
         var _element$ownerDocumen;
-        var html2 = getDocumentElement$2(element2);
-        var winScroll = getWindowScroll$1(element2);
+        var html2 = getDocumentElement(element2);
+        var winScroll = getWindowScroll(element2);
         var body = (_element$ownerDocumen = element2.ownerDocument) == null ? void 0 : _element$ownerDocumen.body;
-        var width = max$4(html2.scrollWidth, html2.clientWidth, body ? body.scrollWidth : 0, body ? body.clientWidth : 0);
-        var height = max$4(html2.scrollHeight, html2.clientHeight, body ? body.scrollHeight : 0, body ? body.clientHeight : 0);
-        var x2 = -winScroll.scrollLeft + getWindowScrollBarX$2(element2);
+        var width = max$3(html2.scrollWidth, html2.clientWidth, body ? body.scrollWidth : 0, body ? body.clientWidth : 0);
+        var height = max$3(html2.scrollHeight, html2.clientHeight, body ? body.scrollHeight : 0, body ? body.clientHeight : 0);
+        var x2 = -winScroll.scrollLeft + getWindowScrollBarX(element2);
         var y2 = -winScroll.scrollTop;
-        if (getComputedStyle$3(body || html2).direction === "rtl") {
-            x2 += max$4(html2.clientWidth, body ? body.clientWidth : 0) - width;
+        if (getComputedStyle$1(body || html2).direction === "rtl") {
+            x2 += max$3(html2.clientWidth, body ? body.clientWidth : 0) - width;
         }
         return {
             width,
             height,
             x: x2,
             y: y2
         };
     }
 
-    function isScrollParent$1(element2) {
-        var _getComputedStyle = getComputedStyle$3(element2),
+    function isScrollParent(element2) {
+        var _getComputedStyle = getComputedStyle$1(element2),
             overflow = _getComputedStyle.overflow,
             overflowX = _getComputedStyle.overflowX,
             overflowY = _getComputedStyle.overflowY;
         return /auto|scroll|overlay|hidden/.test(overflow + overflowY + overflowX);
     }
 
-    function getScrollParent$1(node2) {
-        if (["html", "body", "#document"].indexOf(getNodeName$2(node2)) >= 0) {
+    function getScrollParent(node2) {
+        if (["html", "body", "#document"].indexOf(getNodeName(node2)) >= 0) {
             return node2.ownerDocument.body;
         }
-        if (isHTMLElement$2(node2) && isScrollParent$1(node2)) {
+        if (isHTMLElement(node2) && isScrollParent(node2)) {
             return node2;
         }
-        return getScrollParent$1(getParentNode$2(node2));
+        return getScrollParent(getParentNode(node2));
     }
 
-    function listScrollParents$1(element2, list2) {
+    function listScrollParents(element2, list2) {
         var _element$ownerDocumen;
         if (list2 === void 0) {
             list2 = [];
         }
-        var scrollParent = getScrollParent$1(element2);
+        var scrollParent = getScrollParent(element2);
         var isBody = scrollParent === ((_element$ownerDocumen = element2.ownerDocument) == null ? void 0 : _element$ownerDocumen.body);
-        var win = getWindow$2(scrollParent);
-        var target = isBody ? [win].concat(win.visualViewport || [], isScrollParent$1(scrollParent) ? scrollParent : []) : scrollParent;
+        var win = getWindow(scrollParent);
+        var target = isBody ? [win].concat(win.visualViewport || [], isScrollParent(scrollParent) ? scrollParent : []) : scrollParent;
         var updatedList = list2.concat(target);
-        return isBody ? updatedList : updatedList.concat(listScrollParents$1(getParentNode$2(target)));
+        return isBody ? updatedList : updatedList.concat(listScrollParents(getParentNode(target)));
     }
 
-    function rectToClientRect$2(rect) {
+    function rectToClientRect(rect) {
         return Object.assign({}, rect, {
             left: rect.x,
             top: rect.y,
             right: rect.x + rect.width,
             bottom: rect.y + rect.height
         });
     }
 
-    function getInnerBoundingClientRect$1(element2, strategy) {
-        var rect = getBoundingClientRect$2(element2, false, strategy === "fixed");
+    function getInnerBoundingClientRect(element2, strategy) {
+        var rect = getBoundingClientRect(element2, false, strategy === "fixed");
         rect.top = rect.top + element2.clientTop;
         rect.left = rect.left + element2.clientLeft;
         rect.bottom = rect.top + element2.clientHeight;
         rect.right = rect.left + element2.clientWidth;
         rect.width = element2.clientWidth;
         rect.height = element2.clientHeight;
         rect.x = rect.left;
         rect.y = rect.top;
         return rect;
     }
 
-    function getClientRectFromMixedType$1(element2, clippingParent, strategy) {
-        return clippingParent === viewport$1 ? rectToClientRect$2(getViewportRect$2(element2, strategy)) : isElement$5(clippingParent) ? getInnerBoundingClientRect$1(clippingParent, strategy) : rectToClientRect$2(getDocumentRect$2(getDocumentElement$2(element2)));
+    function getClientRectFromMixedType(element2, clippingParent, strategy) {
+        return clippingParent === viewport ? rectToClientRect(getViewportRect(element2, strategy)) : isElement$3(clippingParent) ? getInnerBoundingClientRect(clippingParent, strategy) : rectToClientRect(getDocumentRect(getDocumentElement(element2)));
     }
 
-    function getClippingParents$1(element2) {
-        var clippingParents2 = listScrollParents$1(getParentNode$2(element2));
-        var canEscapeClipping = ["absolute", "fixed"].indexOf(getComputedStyle$3(element2).position) >= 0;
-        var clipperElement = canEscapeClipping && isHTMLElement$2(element2) ? getOffsetParent$2(element2) : element2;
-        if (!isElement$5(clipperElement)) {
+    function getClippingParents(element2) {
+        var clippingParents2 = listScrollParents(getParentNode(element2));
+        var canEscapeClipping = ["absolute", "fixed"].indexOf(getComputedStyle$1(element2).position) >= 0;
+        var clipperElement = canEscapeClipping && isHTMLElement(element2) ? getOffsetParent(element2) : element2;
+        if (!isElement$3(clipperElement)) {
             return [];
         }
         return clippingParents2.filter(function(clippingParent) {
-            return isElement$5(clippingParent) && contains$2(clippingParent, clipperElement) && getNodeName$2(clippingParent) !== "body";
+            return isElement$3(clippingParent) && contains$1(clippingParent, clipperElement) && getNodeName(clippingParent) !== "body";
         });
     }
 
-    function getClippingRect$2(element2, boundary, rootBoundary, strategy) {
-        var mainClippingParents = boundary === "clippingParents" ? getClippingParents$1(element2) : [].concat(boundary);
+    function getClippingRect(element2, boundary, rootBoundary, strategy) {
+        var mainClippingParents = boundary === "clippingParents" ? getClippingParents(element2) : [].concat(boundary);
         var clippingParents2 = [].concat(mainClippingParents, [rootBoundary]);
         var firstClippingParent = clippingParents2[0];
         var clippingRect = clippingParents2.reduce(function(accRect, clippingParent) {
-            var rect = getClientRectFromMixedType$1(element2, clippingParent, strategy);
-            accRect.top = max$4(rect.top, accRect.top);
-            accRect.right = min$3(rect.right, accRect.right);
-            accRect.bottom = min$3(rect.bottom, accRect.bottom);
-            accRect.left = max$4(rect.left, accRect.left);
+            var rect = getClientRectFromMixedType(element2, clippingParent, strategy);
+            accRect.top = max$3(rect.top, accRect.top);
+            accRect.right = min$2(rect.right, accRect.right);
+            accRect.bottom = min$2(rect.bottom, accRect.bottom);
+            accRect.left = max$3(rect.left, accRect.left);
             return accRect;
-        }, getClientRectFromMixedType$1(element2, firstClippingParent, strategy));
+        }, getClientRectFromMixedType(element2, firstClippingParent, strategy));
         clippingRect.width = clippingRect.right - clippingRect.left;
         clippingRect.height = clippingRect.bottom - clippingRect.top;
         clippingRect.x = clippingRect.left;
         clippingRect.y = clippingRect.top;
         return clippingRect;
     }
 
-    function computeOffsets$1(_ref2) {
+    function computeOffsets(_ref2) {
         var reference2 = _ref2.reference,
             element2 = _ref2.element,
             placement = _ref2.placement;
-        var basePlacement = placement ? getBasePlacement$3(placement) : null;
-        var variation = placement ? getVariation$1(placement) : null;
+        var basePlacement = placement ? getBasePlacement$2(placement) : null;
+        var variation = placement ? getVariation(placement) : null;
         var commonX = reference2.x + reference2.width / 2 - element2.width / 2;
         var commonY = reference2.y + reference2.height / 2 - element2.height / 2;
         var offsets;
         switch (basePlacement) {
-            case top$2:
+            case top$1:
                 offsets = {
                     x: commonX,
                     y: reference2.y - element2.height
                 };
                 break;
-            case bottom$1:
+            case bottom:
                 offsets = {
                     x: commonX,
                     y: reference2.y + reference2.height
                 };
                 break;
-            case right$1:
+            case right:
                 offsets = {
                     x: reference2.x + reference2.width,
                     y: commonY
                 };
                 break;
-            case left$1:
+            case left:
                 offsets = {
                     x: reference2.x - element2.width,
                     y: commonY
                 };
                 break;
             default:
                 offsets = {
                     x: reference2.x,
                     y: reference2.y
                 };
         }
-        var mainAxis = basePlacement ? getMainAxisFromPlacement$1(basePlacement) : null;
+        var mainAxis = basePlacement ? getMainAxisFromPlacement(basePlacement) : null;
         if (mainAxis != null) {
             var len = mainAxis === "y" ? "height" : "width";
             switch (variation) {
-                case start$2:
+                case start$1:
                     offsets[mainAxis] = offsets[mainAxis] - (reference2[len] / 2 - element2[len] / 2);
                     break;
-                case end$1:
+                case end:
                     offsets[mainAxis] = offsets[mainAxis] + (reference2[len] / 2 - element2[len] / 2);
                     break;
             }
         }
         return offsets;
     }
 
-    function detectOverflow$2(state, options) {
+    function detectOverflow(state, options) {
         if (options === void 0) {
             options = {};
         }
         var _options = options,
             _options$placement = _options.placement,
             placement = _options$placement === void 0 ? state.placement : _options$placement,
             _options$strategy = _options.strategy,
             strategy = _options$strategy === void 0 ? state.strategy : _options$strategy,
             _options$boundary = _options.boundary,
-            boundary = _options$boundary === void 0 ? clippingParents$1 : _options$boundary,
+            boundary = _options$boundary === void 0 ? clippingParents : _options$boundary,
             _options$rootBoundary = _options.rootBoundary,
-            rootBoundary = _options$rootBoundary === void 0 ? viewport$1 : _options$rootBoundary,
+            rootBoundary = _options$rootBoundary === void 0 ? viewport : _options$rootBoundary,
             _options$elementConte = _options.elementContext,
-            elementContext = _options$elementConte === void 0 ? popper$1 : _options$elementConte,
+            elementContext = _options$elementConte === void 0 ? popper : _options$elementConte,
             _options$altBoundary = _options.altBoundary,
             altBoundary = _options$altBoundary === void 0 ? false : _options$altBoundary,
             _options$padding = _options.padding,
             padding = _options$padding === void 0 ? 0 : _options$padding;
-        var paddingObject = mergePaddingObject$1(typeof padding !== "number" ? padding : expandToHashMap$1(padding, basePlacements$1));
-        var altContext = elementContext === popper$1 ? reference$1 : popper$1;
+        var paddingObject = mergePaddingObject(typeof padding !== "number" ? padding : expandToHashMap(padding, basePlacements));
+        var altContext = elementContext === popper ? reference : popper;
         var popperRect = state.rects.popper;
         var element2 = state.elements[altBoundary ? altContext : elementContext];
-        var clippingClientRect = getClippingRect$2(isElement$5(element2) ? element2 : element2.contextElement || getDocumentElement$2(state.elements.popper), boundary, rootBoundary, strategy);
-        var referenceClientRect = getBoundingClientRect$2(state.elements.reference);
-        var popperOffsets2 = computeOffsets$1({
+        var clippingClientRect = getClippingRect(isElement$3(element2) ? element2 : element2.contextElement || getDocumentElement(state.elements.popper), boundary, rootBoundary, strategy);
+        var referenceClientRect = getBoundingClientRect(state.elements.reference);
+        var popperOffsets2 = computeOffsets({
             reference: referenceClientRect,
             element: popperRect,
             strategy: "absolute",
             placement
         });
-        var popperClientRect = rectToClientRect$2(Object.assign({}, popperRect, popperOffsets2));
-        var elementClientRect = elementContext === popper$1 ? popperClientRect : referenceClientRect;
+        var popperClientRect = rectToClientRect(Object.assign({}, popperRect, popperOffsets2));
+        var elementClientRect = elementContext === popper ? popperClientRect : referenceClientRect;
         var overflowOffsets = {
             top: clippingClientRect.top - elementClientRect.top + paddingObject.top,
             bottom: elementClientRect.bottom - clippingClientRect.bottom + paddingObject.bottom,
             left: clippingClientRect.left - elementClientRect.left + paddingObject.left,
             right: elementClientRect.right - clippingClientRect.right + paddingObject.right
         };
         var offsetData = state.modifiersData.offset;
-        if (elementContext === popper$1 && offsetData) {
+        if (elementContext === popper && offsetData) {
             var offset2 = offsetData[placement];
             Object.keys(overflowOffsets).forEach(function(key) {
-                var multiply = [right$1, bottom$1].indexOf(key) >= 0 ? 1 : -1;
-                var axis = [top$2, bottom$1].indexOf(key) >= 0 ? "y" : "x";
+                var multiply = [right, bottom].indexOf(key) >= 0 ? 1 : -1;
+                var axis = [top$1, bottom].indexOf(key) >= 0 ? "y" : "x";
                 overflowOffsets[key] += offset2[axis] * multiply;
             });
         }
         return overflowOffsets;
     }
 
-    function computeAutoPlacement$1(state, options) {
+    function computeAutoPlacement(state, options) {
         if (options === void 0) {
             options = {};
         }
         var _options = options,
             placement = _options.placement,
             boundary = _options.boundary,
             rootBoundary = _options.rootBoundary,
             padding = _options.padding,
             flipVariations = _options.flipVariations,
             _options$allowedAutoP = _options.allowedAutoPlacements,
-            allowedAutoPlacements = _options$allowedAutoP === void 0 ? placements$2 : _options$allowedAutoP;
-        var variation = getVariation$1(placement);
-        var placements2 = variation ? flipVariations ? variationPlacements$1 : variationPlacements$1.filter(function(placement2) {
-            return getVariation$1(placement2) === variation;
-        }) : basePlacements$1;
-        var allowedPlacements = placements2.filter(function(placement2) {
+            allowedAutoPlacements = _options$allowedAutoP === void 0 ? placements : _options$allowedAutoP;
+        var variation = getVariation(placement);
+        var placements$12 = variation ? flipVariations ? variationPlacements : variationPlacements.filter(function(placement2) {
+            return getVariation(placement2) === variation;
+        }) : basePlacements;
+        var allowedPlacements = placements$12.filter(function(placement2) {
             return allowedAutoPlacements.indexOf(placement2) >= 0;
         });
         if (allowedPlacements.length === 0) {
-            allowedPlacements = placements2;
+            allowedPlacements = placements$12;
         }
         var overflows = allowedPlacements.reduce(function(acc, placement2) {
-            acc[placement2] = detectOverflow$2(state, {
+            acc[placement2] = detectOverflow(state, {
                 placement: placement2,
                 boundary,
                 rootBoundary,
                 padding
-            })[getBasePlacement$3(placement2)];
+            })[getBasePlacement$2(placement2)];
             return acc;
         }, {});
         return Object.keys(overflows).sort(function(a2, b2) {
             return overflows[a2] - overflows[b2];
         });
     }
 
-    function getExpandedFallbackPlacements$1(placement) {
-        if (getBasePlacement$3(placement) === auto$1) {
+    function getExpandedFallbackPlacements(placement) {
+        if (getBasePlacement$2(placement) === auto) {
             return [];
         }
-        var oppositePlacement = getOppositePlacement$2(placement);
-        return [getOppositeVariationPlacement$1(placement), oppositePlacement, getOppositeVariationPlacement$1(oppositePlacement)];
+        var oppositePlacement = getOppositePlacement(placement);
+        return [getOppositeVariationPlacement(placement), oppositePlacement, getOppositeVariationPlacement(oppositePlacement)];
     }
 
-    function flip$4(_ref2) {
+    function flip(_ref2) {
         var state = _ref2.state,
             options = _ref2.options,
             name2 = _ref2.name;
         if (state.modifiersData[name2]._skip) {
             return;
         }
         var _options$mainAxis = options.mainAxis,
@@ -31520,19 +34225,19 @@
             boundary = options.boundary,
             rootBoundary = options.rootBoundary,
             altBoundary = options.altBoundary,
             _options$flipVariatio = options.flipVariations,
             flipVariations = _options$flipVariatio === void 0 ? true : _options$flipVariatio,
             allowedAutoPlacements = options.allowedAutoPlacements;
         var preferredPlacement = state.options.placement;
-        var basePlacement = getBasePlacement$3(preferredPlacement);
+        var basePlacement = getBasePlacement$2(preferredPlacement);
         var isBasePlacement = basePlacement === preferredPlacement;
-        var fallbackPlacements = specifiedFallbackPlacements || (isBasePlacement || !flipVariations ? [getOppositePlacement$2(preferredPlacement)] : getExpandedFallbackPlacements$1(preferredPlacement));
+        var fallbackPlacements = specifiedFallbackPlacements || (isBasePlacement || !flipVariations ? [getOppositePlacement(preferredPlacement)] : getExpandedFallbackPlacements(preferredPlacement));
         var placements2 = [preferredPlacement].concat(fallbackPlacements).reduce(function(acc, placement2) {
-            return acc.concat(getBasePlacement$3(placement2) === auto$1 ? computeAutoPlacement$1(state, {
+            return acc.concat(getBasePlacement$2(placement2) === auto ? computeAutoPlacement(state, {
                 placement: placement2,
                 boundary,
                 rootBoundary,
                 padding,
                 flipVariations,
                 allowedAutoPlacements
             }) : placement2);
@@ -31540,30 +34245,30 @@
         var referenceRect = state.rects.reference;
         var popperRect = state.rects.popper;
         var checksMap = /* @__PURE__ */ new Map();
         var makeFallbackChecks = true;
         var firstFittingPlacement = placements2[0];
         for (var i2 = 0; i2 < placements2.length; i2++) {
             var placement = placements2[i2];
-            var _basePlacement = getBasePlacement$3(placement);
-            var isStartVariation = getVariation$1(placement) === start$2;
-            var isVertical = [top$2, bottom$1].indexOf(_basePlacement) >= 0;
+            var _basePlacement = getBasePlacement$2(placement);
+            var isStartVariation = getVariation(placement) === start$1;
+            var isVertical = [top$1, bottom].indexOf(_basePlacement) >= 0;
             var len = isVertical ? "width" : "height";
-            var overflow = detectOverflow$2(state, {
+            var overflow = detectOverflow(state, {
                 placement,
                 boundary,
                 rootBoundary,
                 altBoundary,
                 padding
             });
-            var mainVariationSide = isVertical ? isStartVariation ? right$1 : left$1 : isStartVariation ? bottom$1 : top$2;
+            var mainVariationSide = isVertical ? isStartVariation ? right : left : isStartVariation ? bottom : top$1;
             if (referenceRect[len] > popperRect[len]) {
-                mainVariationSide = getOppositePlacement$2(mainVariationSide);
+                mainVariationSide = getOppositePlacement(mainVariationSide);
             }
-            var altVariationSide = getOppositePlacement$2(mainVariationSide);
+            var altVariationSide = getOppositePlacement(mainVariationSide);
             var checks2 = [];
             if (checkMainAxis) {
                 checks2.push(overflow[_basePlacement] <= 0);
             }
             if (checkAltAxis) {
                 checks2.push(overflow[mainVariationSide] <= 0, overflow[altVariationSide] <= 0);
             }
@@ -31600,150 +34305,150 @@
         }
         if (state.placement !== firstFittingPlacement) {
             state.modifiersData[name2]._skip = true;
             state.placement = firstFittingPlacement;
             state.reset = true;
         }
     }
-    const flip$5 = {
+    const flip$1 = {
         name: "flip",
         enabled: true,
         phase: "main",
-        fn: flip$4,
+        fn: flip,
         requiresIfExists: ["offset"],
         data: {
             _skip: false
         }
     };
 
-    function getSideOffsets$2(overflow, rect, preventedOffsets) {
+    function getSideOffsets(overflow, rect, preventedOffsets) {
         if (preventedOffsets === void 0) {
             preventedOffsets = {
                 x: 0,
                 y: 0
             };
         }
         return {
             top: overflow.top - rect.height - preventedOffsets.y,
             right: overflow.right - rect.width + preventedOffsets.x,
             bottom: overflow.bottom - rect.height + preventedOffsets.y,
             left: overflow.left - rect.width - preventedOffsets.x
         };
     }
 
-    function isAnySideFullyClipped$2(overflow) {
-        return [top$2, right$1, bottom$1, left$1].some(function(side) {
+    function isAnySideFullyClipped(overflow) {
+        return [top$1, right, bottom, left].some(function(side) {
             return overflow[side] >= 0;
         });
     }
 
-    function hide$3(_ref2) {
+    function hide(_ref2) {
         var state = _ref2.state,
             name2 = _ref2.name;
         var referenceRect = state.rects.reference;
         var popperRect = state.rects.popper;
         var preventedOffsets = state.modifiersData.preventOverflow;
-        var referenceOverflow = detectOverflow$2(state, {
+        var referenceOverflow = detectOverflow(state, {
             elementContext: "reference"
         });
-        var popperAltOverflow = detectOverflow$2(state, {
+        var popperAltOverflow = detectOverflow(state, {
             altBoundary: true
         });
-        var referenceClippingOffsets = getSideOffsets$2(referenceOverflow, referenceRect);
-        var popperEscapeOffsets = getSideOffsets$2(popperAltOverflow, popperRect, preventedOffsets);
-        var isReferenceHidden = isAnySideFullyClipped$2(referenceClippingOffsets);
-        var hasPopperEscaped = isAnySideFullyClipped$2(popperEscapeOffsets);
+        var referenceClippingOffsets = getSideOffsets(referenceOverflow, referenceRect);
+        var popperEscapeOffsets = getSideOffsets(popperAltOverflow, popperRect, preventedOffsets);
+        var isReferenceHidden = isAnySideFullyClipped(referenceClippingOffsets);
+        var hasPopperEscaped = isAnySideFullyClipped(popperEscapeOffsets);
         state.modifiersData[name2] = {
             referenceClippingOffsets,
             popperEscapeOffsets,
             isReferenceHidden,
             hasPopperEscaped
         };
         state.attributes.popper = Object.assign({}, state.attributes.popper, {
             "data-popper-reference-hidden": isReferenceHidden,
             "data-popper-escaped": hasPopperEscaped
         });
     }
-    const hide$4 = {
+    const hide$1 = {
         name: "hide",
         enabled: true,
         phase: "main",
         requiresIfExists: ["preventOverflow"],
-        fn: hide$3
+        fn: hide
     };
 
-    function distanceAndSkiddingToXY$1(placement, rects, offset2) {
-        var basePlacement = getBasePlacement$3(placement);
-        var invertDistance = [left$1, top$2].indexOf(basePlacement) >= 0 ? -1 : 1;
+    function distanceAndSkiddingToXY(placement, rects, offset2) {
+        var basePlacement = getBasePlacement$2(placement);
+        var invertDistance = [left, top$1].indexOf(basePlacement) >= 0 ? -1 : 1;
         var _ref2 = typeof offset2 === "function" ? offset2(Object.assign({}, rects, {
                 placement
             })) : offset2,
             skidding = _ref2[0],
             distance = _ref2[1];
         skidding = skidding || 0;
         distance = (distance || 0) * invertDistance;
-        return [left$1, right$1].indexOf(basePlacement) >= 0 ? {
+        return [left, right].indexOf(basePlacement) >= 0 ? {
             x: distance,
             y: skidding
         } : {
             x: skidding,
             y: distance
         };
     }
 
-    function offset$2(_ref2) {
+    function offset(_ref2) {
         var state = _ref2.state,
             options = _ref2.options,
             name2 = _ref2.name;
         var _options$offset = options.offset,
             offset2 = _options$offset === void 0 ? [0, 0] : _options$offset;
-        var data2 = placements$2.reduce(function(acc, placement) {
-            acc[placement] = distanceAndSkiddingToXY$1(placement, state.rects, offset2);
+        var data2 = placements.reduce(function(acc, placement) {
+            acc[placement] = distanceAndSkiddingToXY(placement, state.rects, offset2);
             return acc;
         }, {});
         var _data$state$placement = data2[state.placement],
             x2 = _data$state$placement.x,
             y2 = _data$state$placement.y;
         if (state.modifiersData.popperOffsets != null) {
             state.modifiersData.popperOffsets.x += x2;
             state.modifiersData.popperOffsets.y += y2;
         }
         state.modifiersData[name2] = data2;
     }
-    const offset$3 = {
+    const offset$1 = {
         name: "offset",
         enabled: true,
         phase: "main",
         requires: ["popperOffsets"],
-        fn: offset$2
+        fn: offset
     };
 
-    function popperOffsets$2(_ref2) {
+    function popperOffsets(_ref2) {
         var state = _ref2.state,
             name2 = _ref2.name;
-        state.modifiersData[name2] = computeOffsets$1({
+        state.modifiersData[name2] = computeOffsets({
             reference: state.rects.reference,
             element: state.rects.popper,
             strategy: "absolute",
             placement: state.placement
         });
     }
-    const popperOffsets$3 = {
+    const popperOffsets$1 = {
         name: "popperOffsets",
         enabled: true,
         phase: "read",
-        fn: popperOffsets$2,
+        fn: popperOffsets,
         data: {}
     };
 
-    function getAltAxis$1(axis) {
+    function getAltAxis(axis) {
         return axis === "x" ? "y" : "x";
     }
 
-    function preventOverflow$2(_ref2) {
+    function preventOverflow(_ref2) {
         var state = _ref2.state,
             options = _ref2.options,
             name2 = _ref2.name;
         var _options$mainAxis = options.mainAxis,
             checkMainAxis = _options$mainAxis === void 0 ? true : _options$mainAxis,
             _options$altAxis = options.altAxis,
             checkAltAxis = _options$altAxis === void 0 ? false : _options$altAxis,
@@ -31751,25 +34456,25 @@
             rootBoundary = options.rootBoundary,
             altBoundary = options.altBoundary,
             padding = options.padding,
             _options$tether = options.tether,
             tether = _options$tether === void 0 ? true : _options$tether,
             _options$tetherOffset = options.tetherOffset,
             tetherOffset = _options$tetherOffset === void 0 ? 0 : _options$tetherOffset;
-        var overflow = detectOverflow$2(state, {
+        var overflow = detectOverflow(state, {
             boundary,
             rootBoundary,
             padding,
             altBoundary
         });
-        var basePlacement = getBasePlacement$3(state.placement);
-        var variation = getVariation$1(state.placement);
+        var basePlacement = getBasePlacement$2(state.placement);
+        var variation = getVariation(state.placement);
         var isBasePlacement = !variation;
-        var mainAxis = getMainAxisFromPlacement$1(basePlacement);
-        var altAxis = getAltAxis$1(mainAxis);
+        var mainAxis = getMainAxisFromPlacement(basePlacement);
+        var altAxis = getAltAxis(mainAxis);
         var popperOffsets2 = state.modifiersData.popperOffsets;
         var referenceRect = state.rects.reference;
         var popperRect = state.rects.popper;
         var tetherOffsetValue = typeof tetherOffset === "function" ? tetherOffset(Object.assign({}, state.rects, {
             placement: state.placement
         })) : tetherOffset;
         var normalizedTetherOffsetValue = typeof tetherOffsetValue === "number" ? {
@@ -31785,128 +34490,128 @@
             y: 0
         };
         if (!popperOffsets2) {
             return;
         }
         if (checkMainAxis) {
             var _offsetModifierState$;
-            var mainSide = mainAxis === "y" ? top$2 : left$1;
-            var altSide = mainAxis === "y" ? bottom$1 : right$1;
+            var mainSide = mainAxis === "y" ? top$1 : left;
+            var altSide = mainAxis === "y" ? bottom : right;
             var len = mainAxis === "y" ? "height" : "width";
             var offset2 = popperOffsets2[mainAxis];
             var min2 = offset2 + overflow[mainSide];
             var max2 = offset2 - overflow[altSide];
             var additive = tether ? -popperRect[len] / 2 : 0;
-            var minLen = variation === start$2 ? referenceRect[len] : popperRect[len];
-            var maxLen = variation === start$2 ? -popperRect[len] : -referenceRect[len];
+            var minLen = variation === start$1 ? referenceRect[len] : popperRect[len];
+            var maxLen = variation === start$1 ? -popperRect[len] : -referenceRect[len];
             var arrowElement = state.elements.arrow;
-            var arrowRect = tether && arrowElement ? getLayoutRect$1(arrowElement) : {
+            var arrowRect = tether && arrowElement ? getLayoutRect(arrowElement) : {
                 width: 0,
                 height: 0
             };
-            var arrowPaddingObject = state.modifiersData["arrow#persistent"] ? state.modifiersData["arrow#persistent"].padding : getFreshSideObject$1();
+            var arrowPaddingObject = state.modifiersData["arrow#persistent"] ? state.modifiersData["arrow#persistent"].padding : getFreshSideObject();
             var arrowPaddingMin = arrowPaddingObject[mainSide];
             var arrowPaddingMax = arrowPaddingObject[altSide];
-            var arrowLen = within$1(0, referenceRect[len], arrowRect[len]);
+            var arrowLen = within(0, referenceRect[len], arrowRect[len]);
             var minOffset = isBasePlacement ? referenceRect[len] / 2 - additive - arrowLen - arrowPaddingMin - normalizedTetherOffsetValue.mainAxis : minLen - arrowLen - arrowPaddingMin - normalizedTetherOffsetValue.mainAxis;
             var maxOffset2 = isBasePlacement ? -referenceRect[len] / 2 + additive + arrowLen + arrowPaddingMax + normalizedTetherOffsetValue.mainAxis : maxLen + arrowLen + arrowPaddingMax + normalizedTetherOffsetValue.mainAxis;
-            var arrowOffsetParent = state.elements.arrow && getOffsetParent$2(state.elements.arrow);
+            var arrowOffsetParent = state.elements.arrow && getOffsetParent(state.elements.arrow);
             var clientOffset = arrowOffsetParent ? mainAxis === "y" ? arrowOffsetParent.clientTop || 0 : arrowOffsetParent.clientLeft || 0 : 0;
             var offsetModifierValue = (_offsetModifierState$ = offsetModifierState == null ? void 0 : offsetModifierState[mainAxis]) != null ? _offsetModifierState$ : 0;
             var tetherMin = offset2 + minOffset - offsetModifierValue - clientOffset;
             var tetherMax = offset2 + maxOffset2 - offsetModifierValue;
-            var preventedOffset = within$1(tether ? min$3(min2, tetherMin) : min2, offset2, tether ? max$4(max2, tetherMax) : max2);
+            var preventedOffset = within(tether ? min$2(min2, tetherMin) : min2, offset2, tether ? max$3(max2, tetherMax) : max2);
             popperOffsets2[mainAxis] = preventedOffset;
             data2[mainAxis] = preventedOffset - offset2;
         }
         if (checkAltAxis) {
             var _offsetModifierState$2;
-            var _mainSide = mainAxis === "x" ? top$2 : left$1;
-            var _altSide = mainAxis === "x" ? bottom$1 : right$1;
+            var _mainSide = mainAxis === "x" ? top$1 : left;
+            var _altSide = mainAxis === "x" ? bottom : right;
             var _offset = popperOffsets2[altAxis];
             var _len = altAxis === "y" ? "height" : "width";
             var _min = _offset + overflow[_mainSide];
             var _max = _offset - overflow[_altSide];
-            var isOriginSide = [top$2, left$1].indexOf(basePlacement) !== -1;
+            var isOriginSide = [top$1, left].indexOf(basePlacement) !== -1;
             var _offsetModifierValue = (_offsetModifierState$2 = offsetModifierState == null ? void 0 : offsetModifierState[altAxis]) != null ? _offsetModifierState$2 : 0;
             var _tetherMin = isOriginSide ? _min : _offset - referenceRect[_len] - popperRect[_len] - _offsetModifierValue + normalizedTetherOffsetValue.altAxis;
             var _tetherMax = isOriginSide ? _offset + referenceRect[_len] + popperRect[_len] - _offsetModifierValue - normalizedTetherOffsetValue.altAxis : _max;
-            var _preventedOffset = tether && isOriginSide ? withinMaxClamp(_tetherMin, _offset, _tetherMax) : within$1(tether ? _tetherMin : _min, _offset, tether ? _tetherMax : _max);
+            var _preventedOffset = tether && isOriginSide ? withinMaxClamp(_tetherMin, _offset, _tetherMax) : within(tether ? _tetherMin : _min, _offset, tether ? _tetherMax : _max);
             popperOffsets2[altAxis] = _preventedOffset;
             data2[altAxis] = _preventedOffset - _offset;
         }
         state.modifiersData[name2] = data2;
     }
-    const preventOverflow$3 = {
+    const preventOverflow$1 = {
         name: "preventOverflow",
         enabled: true,
         phase: "main",
-        fn: preventOverflow$2,
+        fn: preventOverflow,
         requiresIfExists: ["offset"]
     };
 
-    function getHTMLElementScroll$1(element2) {
+    function getHTMLElementScroll(element2) {
         return {
             scrollLeft: element2.scrollLeft,
             scrollTop: element2.scrollTop
         };
     }
 
-    function getNodeScroll$2(node2) {
-        if (node2 === getWindow$2(node2) || !isHTMLElement$2(node2)) {
-            return getWindowScroll$1(node2);
+    function getNodeScroll(node2) {
+        if (node2 === getWindow(node2) || !isHTMLElement(node2)) {
+            return getWindowScroll(node2);
         } else {
-            return getHTMLElementScroll$1(node2);
+            return getHTMLElementScroll(node2);
         }
     }
 
     function isElementScaled(element2) {
         var rect = element2.getBoundingClientRect();
-        var scaleX = round$3(rect.width) / element2.offsetWidth || 1;
-        var scaleY = round$3(rect.height) / element2.offsetHeight || 1;
+        var scaleX = round$2(rect.width) / element2.offsetWidth || 1;
+        var scaleY = round$2(rect.height) / element2.offsetHeight || 1;
         return scaleX !== 1 || scaleY !== 1;
     }
 
-    function getCompositeRect$1(elementOrVirtualElement, offsetParent, isFixed) {
+    function getCompositeRect(elementOrVirtualElement, offsetParent, isFixed) {
         if (isFixed === void 0) {
             isFixed = false;
         }
-        var isOffsetParentAnElement = isHTMLElement$2(offsetParent);
-        var offsetParentIsScaled = isHTMLElement$2(offsetParent) && isElementScaled(offsetParent);
-        var documentElement = getDocumentElement$2(offsetParent);
-        var rect = getBoundingClientRect$2(elementOrVirtualElement, offsetParentIsScaled, isFixed);
+        var isOffsetParentAnElement = isHTMLElement(offsetParent);
+        var offsetParentIsScaled = isHTMLElement(offsetParent) && isElementScaled(offsetParent);
+        var documentElement = getDocumentElement(offsetParent);
+        var rect = getBoundingClientRect(elementOrVirtualElement, offsetParentIsScaled, isFixed);
         var scroll = {
             scrollLeft: 0,
             scrollTop: 0
         };
         var offsets = {
             x: 0,
             y: 0
         };
         if (isOffsetParentAnElement || !isOffsetParentAnElement && !isFixed) {
-            if (getNodeName$2(offsetParent) !== "body" || isScrollParent$1(documentElement)) {
-                scroll = getNodeScroll$2(offsetParent);
+            if (getNodeName(offsetParent) !== "body" || isScrollParent(documentElement)) {
+                scroll = getNodeScroll(offsetParent);
             }
-            if (isHTMLElement$2(offsetParent)) {
-                offsets = getBoundingClientRect$2(offsetParent, true);
+            if (isHTMLElement(offsetParent)) {
+                offsets = getBoundingClientRect(offsetParent, true);
                 offsets.x += offsetParent.clientLeft;
                 offsets.y += offsetParent.clientTop;
             } else if (documentElement) {
-                offsets.x = getWindowScrollBarX$2(documentElement);
+                offsets.x = getWindowScrollBarX(documentElement);
             }
         }
         return {
             x: rect.left + scroll.scrollLeft - offsets.x,
             y: rect.top + scroll.scrollTop - offsets.y,
             width: rect.width,
             height: rect.height
         };
     }
 
-    function order$1(modifiers2) {
+    function order(modifiers2) {
         var map2 = /* @__PURE__ */ new Map();
         var visited = /* @__PURE__ */ new Set();
         var result = [];
         modifiers2.forEach(function(modifier) {
             map2.set(modifier.name, modifier);
         });
 
@@ -31927,83 +34632,83 @@
             if (!visited.has(modifier.name)) {
                 sort(modifier);
             }
         });
         return result;
     }
 
-    function orderModifiers$1(modifiers2) {
-        var orderedModifiers = order$1(modifiers2);
-        return modifierPhases$1.reduce(function(acc, phase) {
+    function orderModifiers(modifiers2) {
+        var orderedModifiers = order(modifiers2);
+        return modifierPhases.reduce(function(acc, phase) {
             return acc.concat(orderedModifiers.filter(function(modifier) {
                 return modifier.phase === phase;
             }));
         }, []);
     }
 
-    function debounce$5(fn2) {
+    function debounce$4(fn2) {
         var pending;
         return function() {
             if (!pending) {
                 pending = new Promise(function(resolve2) {
                     Promise.resolve().then(function() {
                         pending = void 0;
                         resolve2(fn2());
                     });
                 });
             }
             return pending;
         };
     }
 
-    function mergeByName$1(modifiers2) {
+    function mergeByName(modifiers2) {
         var merged = modifiers2.reduce(function(merged2, current2) {
             var existing = merged2[current2.name];
             merged2[current2.name] = existing ? Object.assign({}, existing, current2, {
                 options: Object.assign({}, existing.options, current2.options),
                 data: Object.assign({}, existing.data, current2.data)
             }) : current2;
             return merged2;
         }, {});
         return Object.keys(merged).map(function(key) {
             return merged[key];
         });
     }
-    var DEFAULT_OPTIONS$2 = {
+    var DEFAULT_OPTIONS$1 = {
         placement: "bottom",
         modifiers: [],
         strategy: "absolute"
     };
 
-    function areValidElements$1() {
+    function areValidElements() {
         for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {
             args[_key] = arguments[_key];
         }
         return !args.some(function(element2) {
             return !(element2 && typeof element2.getBoundingClientRect === "function");
         });
     }
 
-    function popperGenerator$1(generatorOptions) {
+    function popperGenerator(generatorOptions) {
         if (generatorOptions === void 0) {
             generatorOptions = {};
         }
         var _generatorOptions = generatorOptions,
             _generatorOptions$def = _generatorOptions.defaultModifiers,
             defaultModifiers2 = _generatorOptions$def === void 0 ? [] : _generatorOptions$def,
             _generatorOptions$def2 = _generatorOptions.defaultOptions,
-            defaultOptions2 = _generatorOptions$def2 === void 0 ? DEFAULT_OPTIONS$2 : _generatorOptions$def2;
+            defaultOptions2 = _generatorOptions$def2 === void 0 ? DEFAULT_OPTIONS$1 : _generatorOptions$def2;
         return function createPopper2(reference2, popper2, options) {
             if (options === void 0) {
                 options = defaultOptions2;
             }
             var state = {
                 placement: "bottom",
                 orderedModifiers: [],
-                options: Object.assign({}, DEFAULT_OPTIONS$2, defaultOptions2),
+                options: Object.assign({}, DEFAULT_OPTIONS$1, defaultOptions2),
                 modifiersData: {},
                 elements: {
                     reference: reference2,
                     popper: popper2
                 },
                 attributes: {},
                 styles: {}
@@ -32013,37 +34718,37 @@
             var instance2 = {
                 state,
                 setOptions: function setOptions2(setOptionsAction) {
                     var options2 = typeof setOptionsAction === "function" ? setOptionsAction(state.options) : setOptionsAction;
                     cleanupModifierEffects();
                     state.options = Object.assign({}, defaultOptions2, state.options, options2);
                     state.scrollParents = {
-                        reference: isElement$5(reference2) ? listScrollParents$1(reference2) : reference2.contextElement ? listScrollParents$1(reference2.contextElement) : [],
-                        popper: listScrollParents$1(popper2)
+                        reference: isElement$3(reference2) ? listScrollParents(reference2) : reference2.contextElement ? listScrollParents(reference2.contextElement) : [],
+                        popper: listScrollParents(popper2)
                     };
-                    var orderedModifiers = orderModifiers$1(mergeByName$1([].concat(defaultModifiers2, state.options.modifiers)));
+                    var orderedModifiers = orderModifiers(mergeByName([].concat(defaultModifiers2, state.options.modifiers)));
                     state.orderedModifiers = orderedModifiers.filter(function(m2) {
                         return m2.enabled;
                     });
                     runModifierEffects();
                     return instance2.update();
                 },
                 forceUpdate: function forceUpdate() {
                     if (isDestroyed) {
                         return;
                     }
                     var _state$elements = state.elements,
                         reference3 = _state$elements.reference,
                         popper3 = _state$elements.popper;
-                    if (!areValidElements$1(reference3, popper3)) {
+                    if (!areValidElements(reference3, popper3)) {
                         return;
                     }
                     state.rects = {
-                        reference: getCompositeRect$1(reference3, getOffsetParent$2(popper3), state.options.strategy === "fixed"),
-                        popper: getLayoutRect$1(popper3)
+                        reference: getCompositeRect(reference3, getOffsetParent(popper3), state.options.strategy === "fixed"),
+                        popper: getLayoutRect(popper3)
                     };
                     state.reset = false;
                     state.placement = state.options.placement;
                     state.orderedModifiers.forEach(function(modifier) {
                         return state.modifiersData[modifier.name] = Object.assign({}, modifier.data);
                     });
                     for (var index2 = 0; index2 < state.orderedModifiers.length; index2++) {
@@ -32063,26 +34768,26 @@
                                 options: _options,
                                 name: name2,
                                 instance: instance2
                             }) || state;
                         }
                     }
                 },
-                update: debounce$5(function() {
+                update: debounce$4(function() {
                     return new Promise(function(resolve2) {
                         instance2.forceUpdate();
                         resolve2(state);
                     });
                 }),
                 destroy: function destroy() {
                     cleanupModifierEffects();
                     isDestroyed = true;
                 }
             };
-            if (!areValidElements$1(reference2, popper2)) {
+            if (!areValidElements(reference2, popper2)) {
                 return instance2;
             }
             instance2.setOptions(options).then(function(state2) {
                 if (!isDestroyed && options.onFirstUpdate) {
                     options.onFirstUpdate(state2);
                 }
             });
@@ -32111,17 +34816,17 @@
                     return fn2();
                 });
                 effectCleanupFns = [];
             }
             return instance2;
         };
     }
-    var defaultModifiers$1 = [eventListeners$1, popperOffsets$3, computeStyles$3, applyStyles$3, offset$3, flip$5, preventOverflow$3, arrow$4, hide$4];
-    var createPopper$1 = /* @__PURE__ */ popperGenerator$1({
-        defaultModifiers: defaultModifiers$1
+    var defaultModifiers = [eventListeners, popperOffsets$1, computeStyles$1, applyStyles$1, offset$1, flip$1, preventOverflow$1, arrow$1, hide$1];
+    var createPopper = /* @__PURE__ */ popperGenerator({
+        defaultModifiers
     });
     var CONTENT_CLASS$1 = "tippy-content";
     var BACKDROP_CLASS$1 = "tippy-backdrop";
     var ARROW_CLASS$1 = "tippy-arrow";
     var SVG_ARROW_CLASS$1 = "tippy-svg-arrow";
     var TOUCH_OPTIONS$1 = {
         passive: true,
@@ -32141,15 +34846,15 @@
         return str.indexOf("[object") === 0 && str.indexOf(type2 + "]") > -1;
     }
 
     function invokeWithArgsOrReturn$1(value, args) {
         return typeof value === "function" ? value.apply(void 0, args) : value;
     }
 
-    function debounce$4(fn2, ms2) {
+    function debounce$3(fn2, ms2) {
         if (ms2 === 0) {
             return fn2;
         }
         var timeout2;
         return function(arg) {
             clearTimeout(timeout2);
             timeout2 = setTimeout(function() {
@@ -32174,15 +34879,15 @@
 
     function unique$1(arr) {
         return arr.filter(function(item, index2) {
             return arr.indexOf(item) === index2;
         });
     }
 
-    function getBasePlacement$2(placement) {
+    function getBasePlacement$1(placement) {
         return placement.split("-")[0];
     }
 
     function arrayFrom$1(value) {
         return [].slice.call(value);
     }
 
@@ -32195,15 +34900,15 @@
         }, {});
     }
 
     function div$1() {
         return document.createElement("div");
     }
 
-    function isElement$4(value) {
+    function isElement$2(value) {
         return ["Element", "Fragment"].some(function(type2) {
             return isType$1(value, type2);
         });
     }
 
     function isNodeList$2(value) {
         return isType$1(value, "NodeList");
@@ -32214,15 +34919,15 @@
     }
 
     function isReferenceElement$1(value) {
         return !!(value && value._tippy && value._tippy.reference === value);
     }
 
     function getArrayOfElements$1(value) {
-        if (isElement$4(value)) {
+        if (isElement$2(value)) {
             return [value];
         }
         if (isNodeList$2(value)) {
             return arrayFrom$1(value);
         }
         if (Array.isArray(value)) {
             return value;
@@ -32256,15 +34961,15 @@
         var clientX = event2.clientX,
             clientY = event2.clientY;
         return popperTreeData.every(function(_ref2) {
             var popperRect = _ref2.popperRect,
                 popperState = _ref2.popperState,
                 props = _ref2.props;
             var interactiveBorder = props.interactiveBorder;
-            var basePlacement = getBasePlacement$2(popperState.placement);
+            var basePlacement = getBasePlacement$1(popperState.placement);
             var offsetData = popperState.modifiersData.offset;
             if (!offsetData) {
                 return true;
             }
             var topDistance = basePlacement === "bottom" ? offsetData.top.y : 0;
             var bottomDistance = basePlacement === "top" ? offsetData.bottom.y : 0;
             var leftDistance = basePlacement === "right" ? offsetData.left.x : 0;
@@ -32465,15 +35170,15 @@
         var didHideDueToDocumentMouseDown = false;
         var didTouchMove = false;
         var ignoreOnFirstUpdate = false;
         var lastTriggerEvent;
         var currentTransitionEndListener;
         var onFirstUpdate;
         var listeners = [];
-        var debouncedOnMouseMove = debounce$4(onMouseMove, props.interactiveDebounce);
+        var debouncedOnMouseMove = debounce$3(onMouseMove, props.interactiveDebounce);
         var currentTarget;
         var doc2 = getOwnerDocument$1(props.triggerTarget || reference2);
         var id2 = idCounter$2++;
         var popperInstance = null;
         var plugins2 = unique$1(props.plugins);
         var state = {
             isEnabled: true,
@@ -32916,15 +35621,15 @@
                     options: {
                         element: arrow2,
                         padding: 3
                     }
                 });
             }
             modifiers2.push.apply(modifiers2, (popperOptions == null ? void 0 : popperOptions.modifiers) || []);
-            instance2.popperInstance = createPopper$1(computedReference, popper2, Object.assign({}, popperOptions, {
+            instance2.popperInstance = createPopper(computedReference, popper2, Object.assign({}, popperOptions, {
                 placement,
                 onFirstUpdate,
                 modifiers: modifiers2
             }));
         }
 
         function destroyPopperInstance() {
@@ -33024,15 +35729,15 @@
             var nextProps = evaluateProps$1(reference2, Object.assign({}, instance2.props, {}, partialProps, {
                 ignoreAttributes: true
             }));
             instance2.props = nextProps;
             addListeners();
             if (prevProps.interactiveDebounce !== nextProps.interactiveDebounce) {
                 cleanupInteractiveMouseListeners();
-                debouncedOnMouseMove = debounce$4(onMouseMove, nextProps.interactiveDebounce);
+                debouncedOnMouseMove = debounce$3(onMouseMove, nextProps.interactiveDebounce);
             }
             if (prevProps.triggerTarget && !nextProps.triggerTarget) {
                 normalizeToArray$1(prevProps.triggerTarget).forEach(function(node2) {
                     node2.removeAttribute("aria-expanded");
                 });
             } else if (nextProps.triggerTarget) {
                 reference2.removeAttribute("aria-expanded");
@@ -33212,15 +35917,15 @@
         var instances = elements.reduce(function(acc, reference2) {
             var instance2 = reference2 && createTippy$1(reference2, passedProps);
             if (instance2) {
                 acc.push(instance2);
             }
             return acc;
         }, []);
-        return isElement$4(targets) ? instances[0] : instances;
+        return isElement$2(targets) ? instances[0] : instances;
     }
     tippy$1.defaultProps = defaultProps$6;
     tippy$1.setDefaultProps = setDefaultProps$1;
     tippy$1.currentInput = currentInput$1;
     tippy$1.setDefaultProps({
         animation: false
     });
@@ -33275,15 +35980,15 @@
             popperOptions: Object.assign({}, instanceProps.popperOptions, componentProps.popperOptions, {
                 modifiers: [].concat((((_instanceProps$popper = instanceProps.popperOptions) == null ? void 0 : _instanceProps$popper.modifiers) || []).filter(function(modifier) {
                     return modifier.name.indexOf("tippy") >= 0;
                 }), ((_componentProps$poppe = componentProps.popperOptions) == null ? void 0 : _componentProps$poppe.modifiers) || [])
             })
         });
     }
-    var useIsomorphicLayoutEffect$4 = isBrowser$2 ? React.useLayoutEffect : React.useEffect;
+    var useIsomorphicLayoutEffect$3 = isBrowser$2 ? React.useLayoutEffect : React.useEffect;
 
     function useMutableBox(initialValue) {
         var ref2 = React.useRef();
         if (!ref2.current) {
             ref2.current = typeof initialValue === "function" ? initialValue() : initialValue;
         }
         return ref2.current;
@@ -33392,15 +36097,15 @@
                         return {
                             popper: mutableBox.container
                         };
                     }
                 });
             }
             var deps = [reference2].concat(children2 ? [children2.type] : []);
-            useIsomorphicLayoutEffect$4(function() {
+            useIsomorphicLayoutEffect$3(function() {
                 var element2 = reference2;
                 if (reference2 && reference2.hasOwnProperty("current")) {
                     element2 = reference2.current;
                 }
                 var instance2 = tippy2(element2 || mutableBox.ref || ssrSafeCreateDiv(), Object.assign({}, computedProps, {
                     plugins: [classNamePlugin].concat(props.plugins || [])
                 }));
@@ -33420,15 +36125,15 @@
                 }
                 setMounted(true);
                 return function() {
                     instance2.destroy();
                     singleton == null ? void 0 : singleton.cleanup(instance2);
                 };
             }, deps);
-            useIsomorphicLayoutEffect$4(function() {
+            useIsomorphicLayoutEffect$3(function() {
                 if (mutableBox.renders === 1) {
                     mutableBox.renders++;
                     return;
                 }
                 var instance2 = mutableBox.instance;
                 instance2.setProps(deepPreserveProps(instance2.props, computedProps));
                 if (disabled2) {
@@ -33447,15 +36152,15 @@
                     singleton.hook({
                         instance: instance2,
                         content: content2,
                         props: computedProps
                     });
                 }
             });
-            useIsomorphicLayoutEffect$4(function() {
+            useIsomorphicLayoutEffect$3(function() {
                 var _instance$props$poppe;
                 if (!render2) {
                     return;
                 }
                 var instance2 = mutableBox.instance;
                 instance2.setProps({
                     popperOptions: Object.assign({}, instance2.props.popperOptions, {
@@ -33531,15 +36236,15 @@
         return str.indexOf("[object") === 0 && str.indexOf(type2 + "]") > -1;
     }
 
     function invokeWithArgsOrReturn(value, args) {
         return typeof value === "function" ? value.apply(void 0, args) : value;
     }
 
-    function debounce$3(fn2, ms2) {
+    function debounce$2(fn2, ms2) {
         if (ms2 === 0) {
             return fn2;
         }
         var timeout2;
         return function(arg) {
             clearTimeout(timeout2);
             timeout2 = setTimeout(function() {
@@ -33564,15 +36269,15 @@
 
     function unique(arr) {
         return arr.filter(function(item, index2) {
             return arr.indexOf(item) === index2;
         });
     }
 
-    function getBasePlacement$1(placement) {
+    function getBasePlacement(placement) {
         return placement.split("-")[0];
     }
 
     function arrayFrom(value) {
         return [].slice.call(value);
     }
 
@@ -33585,15 +36290,15 @@
         }, {});
     }
 
     function div() {
         return document.createElement("div");
     }
 
-    function isElement$3(value) {
+    function isElement$1(value) {
         return ["Element", "Fragment"].some(function(type2) {
             return isType(value, type2);
         });
     }
 
     function isNodeList$1(value) {
         return isType(value, "NodeList");
@@ -33604,15 +36309,15 @@
     }
 
     function isReferenceElement(value) {
         return !!(value && value._tippy && value._tippy.reference === value);
     }
 
     function getArrayOfElements(value) {
-        if (isElement$3(value)) {
+        if (isElement$1(value)) {
             return [value];
         }
         if (isNodeList$1(value)) {
             return arrayFrom(value);
         }
         if (Array.isArray(value)) {
             return value;
@@ -33646,15 +36351,15 @@
         var clientX = event2.clientX,
             clientY = event2.clientY;
         return popperTreeData.every(function(_ref2) {
             var popperRect = _ref2.popperRect,
                 popperState = _ref2.popperState,
                 props = _ref2.props;
             var interactiveBorder = props.interactiveBorder;
-            var basePlacement = getBasePlacement$1(popperState.placement);
+            var basePlacement = getBasePlacement(popperState.placement);
             var offsetData = popperState.modifiersData.offset;
             if (!offsetData) {
                 return true;
             }
             var topDistance = basePlacement === "bottom" ? offsetData.top.y : 0;
             var bottomDistance = basePlacement === "top" ? offsetData.bottom.y : 0;
             var leftDistance = basePlacement === "right" ? offsetData.left.x : 0;
@@ -33835,25 +36540,25 @@
 
     function createArrowElement(value) {
         var arrow2 = div();
         if (value === true) {
             arrow2.className = ARROW_CLASS;
         } else {
             arrow2.className = SVG_ARROW_CLASS;
-            if (isElement$3(value)) {
+            if (isElement$1(value)) {
                 arrow2.appendChild(value);
             } else {
                 dangerouslySetInnerHTML(arrow2, value);
             }
         }
         return arrow2;
     }
 
     function setContent(content2, props) {
-        if (isElement$3(props.content)) {
+        if (isElement$1(props.content)) {
             dangerouslySetInnerHTML(content2, "");
             content2.appendChild(props.content);
         } else if (typeof props.content !== "function") {
             if (props.allowHTML) {
                 dangerouslySetInnerHTML(content2, props.content);
             } else {
                 content2.textContent = props.content;
@@ -33951,15 +36656,15 @@
         var didHideDueToDocumentMouseDown = false;
         var didTouchMove = false;
         var ignoreOnFirstUpdate = false;
         var lastTriggerEvent;
         var currentTransitionEndListener;
         var onFirstUpdate;
         var listeners = [];
-        var debouncedOnMouseMove = debounce$3(onMouseMove, props.interactiveDebounce);
+        var debouncedOnMouseMove = debounce$2(onMouseMove, props.interactiveDebounce);
         var currentTarget;
         var doc2 = getOwnerDocument(props.triggerTarget || reference2);
         var id2 = idCounter$1++;
         var popperInstance = null;
         var plugins2 = unique(props.plugins);
         var state = {
             isEnabled: true,
@@ -34402,15 +37107,15 @@
                     options: {
                         element: arrow2,
                         padding: 3
                     }
                 });
             }
             modifiers2.push.apply(modifiers2, (popperOptions == null ? void 0 : popperOptions.modifiers) || []);
-            instance2.popperInstance = createPopper$1(computedReference, popper2, Object.assign({}, popperOptions, {
+            instance2.popperInstance = createPopper(computedReference, popper2, Object.assign({}, popperOptions, {
                 placement,
                 onFirstUpdate,
                 modifiers: modifiers2
             }));
         }
 
         function destroyPopperInstance() {
@@ -34510,15 +37215,15 @@
             var nextProps = evaluateProps(reference2, Object.assign({}, instance2.props, {}, partialProps, {
                 ignoreAttributes: true
             }));
             instance2.props = nextProps;
             addListeners();
             if (prevProps.interactiveDebounce !== nextProps.interactiveDebounce) {
                 cleanupInteractiveMouseListeners();
-                debouncedOnMouseMove = debounce$3(onMouseMove, nextProps.interactiveDebounce);
+                debouncedOnMouseMove = debounce$2(onMouseMove, nextProps.interactiveDebounce);
             }
             if (prevProps.triggerTarget && !nextProps.triggerTarget) {
                 normalizeToArray(prevProps.triggerTarget).forEach(function(node2) {
                     node2.removeAttribute("aria-expanded");
                 });
             } else if (nextProps.triggerTarget) {
                 reference2.removeAttribute("aria-expanded");
@@ -34698,15 +37403,15 @@
         var instances = elements.reduce(function(acc, reference2) {
             var instance2 = reference2 && createTippy(reference2, passedProps);
             if (instance2) {
                 acc.push(instance2);
             }
             return acc;
         }, []);
-        return isElement$3(targets) ? instances[0] : instances;
+        return isElement$1(targets) ? instances[0] : instances;
     }
     tippy.defaultProps = defaultProps$5;
     tippy.setDefaultProps = setDefaultProps;
     tippy.currentInput = currentInput;
     var mouseCoords = {
         clientX: 0,
         clientY: 0
@@ -35239,15 +37944,14 @@
     overflow-y: auto;
     display: flex;
     flex-direction: column;
     gap: 1rem;
 
     width: 350px;
     height: calc(100vh - 2rem);
-    margin: 1rem;
     padding: 1.5rem;
 
     background-color: ${(props) => props.theme.colors.background}e6;
     border-radius: 0.4rem;
     box-shadow: ${(props) => props.theme.shadow.medium};
 `;
     const ReplyWrapper = styled__default.default.div`
@@ -35956,21 +38660,20 @@
         });
     }
 
     function _objectWithoutPropertiesLoose$4(source, excluded) {
         if (source == null)
             return {};
         var target = {};
-        var sourceKeys = Object.keys(source);
-        var key, i2;
-        for (i2 = 0; i2 < sourceKeys.length; i2++) {
-            key = sourceKeys[i2];
-            if (excluded.indexOf(key) >= 0)
-                continue;
-            target[key] = source[key];
+        for (var key in source) {
+            if (Object.prototype.hasOwnProperty.call(source, key)) {
+                if (excluded.indexOf(key) >= 0)
+                    continue;
+                target[key] = source[key];
+            }
         }
         return target;
     }
     var reactIs = {
         exports: {}
     };
     var reactIs_production_min = {};
@@ -36473,15 +39176,15 @@
     }
 
     function isOrContainsNode(parent, child, environment) {
         var result = parent === child || child instanceof environment.Node && parent.contains && parent.contains(child);
         return result;
     }
 
-    function debounce$2(fn2, time) {
+    function debounce$1(fn2, time) {
         var timeoutId;
 
         function cancel() {
             if (timeoutId) {
                 clearTimeout(timeoutId);
             }
         }
@@ -36624,15 +39327,15 @@
         if (checkActiveElement === void 0) {
             checkActiveElement = true;
         }
         return downshiftElements.some(function(contextNode) {
             return contextNode && (isOrContainsNode(contextNode, target, environment) || checkActiveElement && isOrContainsNode(contextNode, environment.document.activeElement, environment));
         });
     }
-    var cleanupStatus = debounce$2(function(documentProp) {
+    var cleanupStatus = debounce$1(function(documentProp) {
         getStatusDiv(documentProp).textContent = "";
     }, 500);
 
     function setStatus(status2, documentProp) {
         var div2 = getStatusDiv(documentProp);
         if (!status2) {
             return;
@@ -36708,18 +39411,18 @@
     }
 
     function getA11ySelectionMessage(selectionParameters) {
         var selectedItem = selectionParameters.selectedItem,
             itemToStringLocal = selectionParameters.itemToString;
         return selectedItem ? itemToStringLocal(selectedItem) + " has been selected." : "";
     }
-    var updateA11yStatus = debounce$2(function(getA11yMessage, document2) {
+    var updateA11yStatus = debounce$1(function(getA11yMessage, document2) {
         setStatus(getA11yMessage(), document2);
     }, 200);
-    var useIsomorphicLayoutEffect$3 = typeof window !== "undefined" && typeof window.document !== "undefined" && typeof window.document.createElement !== "undefined" ? React.useLayoutEffect : React.useEffect;
+    var useIsomorphicLayoutEffect$2 = typeof window !== "undefined" && typeof window.document !== "undefined" && typeof window.document.createElement !== "undefined" ? React.useLayoutEffect : React.useEffect;
 
     function useElementIds(_ref2) {
         var _ref$id = _ref2.id,
             id2 = _ref$id === void 0 ? "downshift-" + generateId() : _ref$id,
             labelId = _ref2.labelId,
             menuId = _ref2.menuId,
             getItemId = _ref2.getItemId,
@@ -36760,15 +39463,15 @@
         return /^\S{1}$/.test(key);
     }
 
     function capitalizeString(string2) {
         return "" + string2.slice(0, 1).toUpperCase() + string2.slice(1);
     }
 
-    function useLatestRef$1(val) {
+    function useLatestRef(val) {
         var ref2 = React.useRef(val);
         ref2.current = val;
         return ref2;
     }
 
     function useEnhancedReducer(reducer2, initialState2, props) {
         var prevStateRef = React.useRef();
@@ -36781,15 +39484,15 @@
                 changes
             }));
             return newState;
         }, [reducer2]);
         var _useReducer = React.useReducer(enhancedReducer, initialState2),
             state = _useReducer[0],
             dispatch2 = _useReducer[1];
-        var propsRef = useLatestRef$1(props);
+        var propsRef = useLatestRef(props);
         var dispatchWithProps = React.useCallback(function(action2) {
             return dispatch2(_extends$3({
                 props: propsRef.current
             }, action2));
         }, [propsRef]);
         var action = actionRef.current;
         React.useEffect(function() {
@@ -36954,15 +39657,15 @@
         var highlightedIndex = _ref3.highlightedIndex,
             isOpen = _ref3.isOpen,
             itemRefs = _ref3.itemRefs,
             getItemNodeFromIndex = _ref3.getItemNodeFromIndex,
             menuElement = _ref3.menuElement,
             scrollIntoViewProp = _ref3.scrollIntoView;
         var shouldScrollRef = React.useRef(true);
-        useIsomorphicLayoutEffect$3(function() {
+        useIsomorphicLayoutEffect$2(function() {
             if (highlightedIndex < 0 || !isOpen || !Object.keys(itemRefs.current).length) {
                 return;
             }
             if (shouldScrollRef.current === false) {
                 shouldScrollRef.current = true;
             } else {
                 scrollIntoViewProp(getItemNodeFromIndex(highlightedIndex), menuElement);
@@ -37295,15 +39998,15 @@
         var toggleButtonRef = React.useRef(null);
         var menuRef = React.useRef(null);
         var itemRefs = React.useRef({});
         var clearTimeoutRef = React.useRef(null);
         var elementIds = useElementIds(props);
         var previousResultCountRef = React.useRef();
         var isInitialMountRef = React.useRef(true);
-        var latest2 = useLatestRef$1({
+        var latest2 = useLatestRef({
             state,
             props
         });
         var getItemNodeFromIndex = React.useCallback(function(index2) {
             return itemRefs.current[elementIds.getItemId(index2)];
         }, [elementIds]);
         useA11yMessageSetter(getA11yStatusMessage2, [isOpen, highlightedIndex, inputValue, items], _extends$3({
@@ -37325,15 +40028,15 @@
             highlightedIndex,
             isOpen,
             itemRefs,
             scrollIntoView: scrollIntoView2,
             getItemNodeFromIndex
         });
         React.useEffect(function() {
-            clearTimeoutRef.current = debounce$2(function(outerDispatch) {
+            clearTimeoutRef.current = debounce$1(function(outerDispatch) {
                 outerDispatch({
                     type: FunctionSetInputValue$1,
                     inputValue: ""
                 });
             }, 500);
             return function() {
                 clearTimeoutRef.current.cancel();
@@ -37916,15 +40619,15 @@
         var menuRef = React.useRef(null);
         var itemRefs = React.useRef({});
         var inputRef = React.useRef(null);
         var toggleButtonRef = React.useRef(null);
         var isInitialMountRef = React.useRef(true);
         var elementIds = useElementIds(props);
         var previousResultCountRef = React.useRef();
-        var latest2 = useLatestRef$1({
+        var latest2 = useLatestRef({
             state,
             props
         });
         var getItemNodeFromIndex = React.useCallback(function(index2) {
             return itemRefs.current[elementIds.getItemId(index2)];
         }, [elementIds]);
         useA11yMessageSetter(getA11yStatusMessage2, [isOpen, highlightedIndex, inputValue, items], _extends$3({
@@ -38496,15 +41199,15 @@
         var activeIndex = state.activeIndex,
             selectedItems = state.selectedItems;
         var isInitialMountRef = React.useRef(true);
         var dropdownRef = React.useRef(null);
         var previousSelectedItemsRef = React.useRef(selectedItems);
         var selectedItemRefs = React.useRef();
         selectedItemRefs.current = [];
-        var latest2 = useLatestRef$1({
+        var latest2 = useLatestRef({
             state,
             props
         });
         React.useEffect(function() {
             if (isInitialMountRef.current || false) {
                 return;
             }
@@ -38683,1547 +41386,14 @@
             setSelectedItems,
             setActiveIndex,
             reset: reset2,
             selectedItems,
             activeIndex
         };
     }
-    var fromEntries$1 = function fromEntries2(entries) {
-        return entries.reduce(function(acc, _ref2) {
-            var key = _ref2[0],
-                value = _ref2[1];
-            acc[key] = value;
-            return acc;
-        }, {});
-    };
-    var useIsomorphicLayoutEffect$2 = typeof window !== "undefined" && window.document && window.document.createElement ? React__namespace.useLayoutEffect : React__namespace.useEffect;
-
-    function getBoundingClientRect$1(element2) {
-        var rect = element2.getBoundingClientRect();
-        return {
-            width: rect.width,
-            height: rect.height,
-            top: rect.top,
-            right: rect.right,
-            bottom: rect.bottom,
-            left: rect.left,
-            x: rect.left,
-            y: rect.top
-        };
-    }
-
-    function getWindow$1(node2) {
-        if (node2.toString() !== "[object Window]") {
-            var ownerDocument = node2.ownerDocument;
-            return ownerDocument ? ownerDocument.defaultView : window;
-        }
-        return node2;
-    }
-
-    function getWindowScroll(node2) {
-        var win = getWindow$1(node2);
-        var scrollLeft = win.pageXOffset;
-        var scrollTop = win.pageYOffset;
-        return {
-            scrollLeft,
-            scrollTop
-        };
-    }
-
-    function isElement$2(node2) {
-        var OwnElement = getWindow$1(node2).Element;
-        return node2 instanceof OwnElement || node2 instanceof Element;
-    }
-
-    function isHTMLElement$1(node2) {
-        var OwnElement = getWindow$1(node2).HTMLElement;
-        return node2 instanceof OwnElement || node2 instanceof HTMLElement;
-    }
-
-    function getHTMLElementScroll(element2) {
-        return {
-            scrollLeft: element2.scrollLeft,
-            scrollTop: element2.scrollTop
-        };
-    }
-
-    function getNodeScroll$1(node2) {
-        if (node2 === getWindow$1(node2) || !isHTMLElement$1(node2)) {
-            return getWindowScroll(node2);
-        } else {
-            return getHTMLElementScroll(node2);
-        }
-    }
-
-    function getNodeName$1(element2) {
-        return element2 ? (element2.nodeName || "").toLowerCase() : null;
-    }
-
-    function getDocumentElement$1(element2) {
-        return (isElement$2(element2) ? element2.ownerDocument : element2.document).documentElement;
-    }
-
-    function getWindowScrollBarX$1(element2) {
-        return getBoundingClientRect$1(getDocumentElement$1(element2)).left + getWindowScroll(element2).scrollLeft;
-    }
-
-    function getComputedStyle$2(element2) {
-        return getWindow$1(element2).getComputedStyle(element2);
-    }
-
-    function isScrollParent(element2) {
-        var _getComputedStyle = getComputedStyle$2(element2),
-            overflow = _getComputedStyle.overflow,
-            overflowX = _getComputedStyle.overflowX,
-            overflowY = _getComputedStyle.overflowY;
-        return /auto|scroll|overlay|hidden/.test(overflow + overflowY + overflowX);
-    }
-
-    function getCompositeRect(elementOrVirtualElement, offsetParent, isFixed) {
-        if (isFixed === void 0) {
-            isFixed = false;
-        }
-        var documentElement = getDocumentElement$1(offsetParent);
-        var rect = getBoundingClientRect$1(elementOrVirtualElement);
-        var scroll = {
-            scrollLeft: 0,
-            scrollTop: 0
-        };
-        var offsets = {
-            x: 0,
-            y: 0
-        };
-        if (!isFixed) {
-            if (getNodeName$1(offsetParent) !== "body" || isScrollParent(documentElement)) {
-                scroll = getNodeScroll$1(offsetParent);
-            }
-            if (isHTMLElement$1(offsetParent)) {
-                offsets = getBoundingClientRect$1(offsetParent);
-                offsets.x += offsetParent.clientLeft;
-                offsets.y += offsetParent.clientTop;
-            } else if (documentElement) {
-                offsets.x = getWindowScrollBarX$1(documentElement);
-            }
-        }
-        return {
-            x: rect.left + scroll.scrollLeft - offsets.x,
-            y: rect.top + scroll.scrollTop - offsets.y,
-            width: rect.width,
-            height: rect.height
-        };
-    }
-
-    function getLayoutRect(element2) {
-        return {
-            x: element2.offsetLeft,
-            y: element2.offsetTop,
-            width: element2.offsetWidth,
-            height: element2.offsetHeight
-        };
-    }
-
-    function getParentNode$1(element2) {
-        if (getNodeName$1(element2) === "html") {
-            return element2;
-        }
-        return element2.assignedSlot || element2.parentNode || element2.host || getDocumentElement$1(element2);
-    }
-
-    function getScrollParent(node2) {
-        if (["html", "body", "#document"].indexOf(getNodeName$1(node2)) >= 0) {
-            return node2.ownerDocument.body;
-        }
-        if (isHTMLElement$1(node2) && isScrollParent(node2)) {
-            return node2;
-        }
-        return getScrollParent(getParentNode$1(node2));
-    }
-
-    function listScrollParents(element2, list2) {
-        if (list2 === void 0) {
-            list2 = [];
-        }
-        var scrollParent = getScrollParent(element2);
-        var isBody = getNodeName$1(scrollParent) === "body";
-        var win = getWindow$1(scrollParent);
-        var target = isBody ? [win].concat(win.visualViewport || [], isScrollParent(scrollParent) ? scrollParent : []) : scrollParent;
-        var updatedList = list2.concat(target);
-        return isBody ? updatedList : updatedList.concat(listScrollParents(getParentNode$1(target)));
-    }
-
-    function isTableElement$1(element2) {
-        return ["table", "td", "th"].indexOf(getNodeName$1(element2)) >= 0;
-    }
-
-    function getTrueOffsetParent$1(element2) {
-        if (!isHTMLElement$1(element2) || getComputedStyle$2(element2).position === "fixed") {
-            return null;
-        }
-        return element2.offsetParent;
-    }
-
-    function getOffsetParent$1(element2) {
-        var window2 = getWindow$1(element2);
-        var offsetParent = getTrueOffsetParent$1(element2);
-        while (offsetParent && isTableElement$1(offsetParent)) {
-            offsetParent = getTrueOffsetParent$1(offsetParent);
-        }
-        if (offsetParent && getNodeName$1(offsetParent) === "body" && getComputedStyle$2(offsetParent).position === "static") {
-            return window2;
-        }
-        return offsetParent || window2;
-    }
-    var top$1 = "top";
-    var bottom = "bottom";
-    var right = "right";
-    var left = "left";
-    var auto = "auto";
-    var basePlacements = [top$1, bottom, right, left];
-    var start$1 = "start";
-    var end = "end";
-    var clippingParents = "clippingParents";
-    var viewport = "viewport";
-    var popper = "popper";
-    var reference = "reference";
-    var variationPlacements = /* @__PURE__ */ basePlacements.reduce(function(acc, placement) {
-        return acc.concat([placement + "-" + start$1, placement + "-" + end]);
-    }, []);
-    var placements$1 = /* @__PURE__ */ [].concat(basePlacements, [auto]).reduce(function(acc, placement) {
-        return acc.concat([placement, placement + "-" + start$1, placement + "-" + end]);
-    }, []);
-    var beforeRead = "beforeRead";
-    var read = "read";
-    var afterRead = "afterRead";
-    var beforeMain = "beforeMain";
-    var main = "main";
-    var afterMain = "afterMain";
-    var beforeWrite = "beforeWrite";
-    var write = "write";
-    var afterWrite = "afterWrite";
-    var modifierPhases = [beforeRead, read, afterRead, beforeMain, main, afterMain, beforeWrite, write, afterWrite];
-
-    function order(modifiers2) {
-        var map2 = /* @__PURE__ */ new Map();
-        var visited = /* @__PURE__ */ new Set();
-        var result = [];
-        modifiers2.forEach(function(modifier) {
-            map2.set(modifier.name, modifier);
-        });
-
-        function sort(modifier) {
-            visited.add(modifier.name);
-            var requires = [].concat(modifier.requires || [], modifier.requiresIfExists || []);
-            requires.forEach(function(dep) {
-                if (!visited.has(dep)) {
-                    var depModifier = map2.get(dep);
-                    if (depModifier) {
-                        sort(depModifier);
-                    }
-                }
-            });
-            result.push(modifier);
-        }
-        modifiers2.forEach(function(modifier) {
-            if (!visited.has(modifier.name)) {
-                sort(modifier);
-            }
-        });
-        return result;
-    }
-
-    function orderModifiers(modifiers2) {
-        var orderedModifiers = order(modifiers2);
-        return modifierPhases.reduce(function(acc, phase) {
-            return acc.concat(orderedModifiers.filter(function(modifier) {
-                return modifier.phase === phase;
-            }));
-        }, []);
-    }
-
-    function debounce$1(fn2) {
-        var pending;
-        return function() {
-            if (!pending) {
-                pending = new Promise(function(resolve2) {
-                    Promise.resolve().then(function() {
-                        pending = void 0;
-                        resolve2(fn2());
-                    });
-                });
-            }
-            return pending;
-        };
-    }
-
-    function getBasePlacement(placement) {
-        return placement.split("-")[0];
-    }
-
-    function mergeByName(modifiers2) {
-        var merged = modifiers2.reduce(function(merged2, current2) {
-            var existing = merged2[current2.name];
-            merged2[current2.name] = existing ? Object.assign({}, existing, {}, current2, {
-                options: Object.assign({}, existing.options, {}, current2.options),
-                data: Object.assign({}, existing.data, {}, current2.data)
-            }) : current2;
-            return merged2;
-        }, {});
-        return Object.keys(merged).map(function(key) {
-            return merged[key];
-        });
-    }
-    var DEFAULT_OPTIONS$1 = {
-        placement: "bottom",
-        modifiers: [],
-        strategy: "absolute"
-    };
-
-    function areValidElements() {
-        for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {
-            args[_key] = arguments[_key];
-        }
-        return !args.some(function(element2) {
-            return !(element2 && typeof element2.getBoundingClientRect === "function");
-        });
-    }
-
-    function popperGenerator(generatorOptions) {
-        if (generatorOptions === void 0) {
-            generatorOptions = {};
-        }
-        var _generatorOptions = generatorOptions,
-            _generatorOptions$def = _generatorOptions.defaultModifiers,
-            defaultModifiers2 = _generatorOptions$def === void 0 ? [] : _generatorOptions$def,
-            _generatorOptions$def2 = _generatorOptions.defaultOptions,
-            defaultOptions2 = _generatorOptions$def2 === void 0 ? DEFAULT_OPTIONS$1 : _generatorOptions$def2;
-        return function createPopper2(reference2, popper2, options) {
-            if (options === void 0) {
-                options = defaultOptions2;
-            }
-            var state = {
-                placement: "bottom",
-                orderedModifiers: [],
-                options: Object.assign({}, DEFAULT_OPTIONS$1, {}, defaultOptions2),
-                modifiersData: {},
-                elements: {
-                    reference: reference2,
-                    popper: popper2
-                },
-                attributes: {},
-                styles: {}
-            };
-            var effectCleanupFns = [];
-            var isDestroyed = false;
-            var instance2 = {
-                state,
-                setOptions: function setOptions2(options2) {
-                    cleanupModifierEffects();
-                    state.options = Object.assign({}, defaultOptions2, {}, state.options, {}, options2);
-                    state.scrollParents = {
-                        reference: isElement$2(reference2) ? listScrollParents(reference2) : reference2.contextElement ? listScrollParents(reference2.contextElement) : [],
-                        popper: listScrollParents(popper2)
-                    };
-                    var orderedModifiers = orderModifiers(mergeByName([].concat(defaultModifiers2, state.options.modifiers)));
-                    state.orderedModifiers = orderedModifiers.filter(function(m2) {
-                        return m2.enabled;
-                    });
-                    runModifierEffects();
-                    return instance2.update();
-                },
-                forceUpdate: function forceUpdate() {
-                    if (isDestroyed) {
-                        return;
-                    }
-                    var _state$elements = state.elements,
-                        reference3 = _state$elements.reference,
-                        popper3 = _state$elements.popper;
-                    if (!areValidElements(reference3, popper3)) {
-                        return;
-                    }
-                    state.rects = {
-                        reference: getCompositeRect(reference3, getOffsetParent$1(popper3), state.options.strategy === "fixed"),
-                        popper: getLayoutRect(popper3)
-                    };
-                    state.reset = false;
-                    state.placement = state.options.placement;
-                    state.orderedModifiers.forEach(function(modifier) {
-                        return state.modifiersData[modifier.name] = Object.assign({}, modifier.data);
-                    });
-                    for (var index2 = 0; index2 < state.orderedModifiers.length; index2++) {
-                        if (state.reset === true) {
-                            state.reset = false;
-                            index2 = -1;
-                            continue;
-                        }
-                        var _state$orderedModifie = state.orderedModifiers[index2],
-                            fn2 = _state$orderedModifie.fn,
-                            _state$orderedModifie2 = _state$orderedModifie.options,
-                            _options = _state$orderedModifie2 === void 0 ? {} : _state$orderedModifie2,
-                            name2 = _state$orderedModifie.name;
-                        if (typeof fn2 === "function") {
-                            state = fn2({
-                                state,
-                                options: _options,
-                                name: name2,
-                                instance: instance2
-                            }) || state;
-                        }
-                    }
-                },
-                update: debounce$1(function() {
-                    return new Promise(function(resolve2) {
-                        instance2.forceUpdate();
-                        resolve2(state);
-                    });
-                }),
-                destroy: function destroy() {
-                    cleanupModifierEffects();
-                    isDestroyed = true;
-                }
-            };
-            if (!areValidElements(reference2, popper2)) {
-                return instance2;
-            }
-            instance2.setOptions(options).then(function(state2) {
-                if (!isDestroyed && options.onFirstUpdate) {
-                    options.onFirstUpdate(state2);
-                }
-            });
-
-            function runModifierEffects() {
-                state.orderedModifiers.forEach(function(_ref3) {
-                    var name2 = _ref3.name,
-                        _ref3$options = _ref3.options,
-                        options2 = _ref3$options === void 0 ? {} : _ref3$options,
-                        effect2 = _ref3.effect;
-                    if (typeof effect2 === "function") {
-                        var cleanupFn = effect2({
-                            state,
-                            name: name2,
-                            instance: instance2,
-                            options: options2
-                        });
-                        var noopFn = function noopFn2() {};
-                        effectCleanupFns.push(cleanupFn || noopFn);
-                    }
-                });
-            }
-
-            function cleanupModifierEffects() {
-                effectCleanupFns.forEach(function(fn2) {
-                    return fn2();
-                });
-                effectCleanupFns = [];
-            }
-            return instance2;
-        };
-    }
-    var passive = {
-        passive: true
-    };
-
-    function effect$2(_ref2) {
-        var state = _ref2.state,
-            instance2 = _ref2.instance,
-            options = _ref2.options;
-        var _options$scroll = options.scroll,
-            scroll = _options$scroll === void 0 ? true : _options$scroll,
-            _options$resize = options.resize,
-            resize = _options$resize === void 0 ? true : _options$resize;
-        var window2 = getWindow$1(state.elements.popper);
-        var scrollParents = [].concat(state.scrollParents.reference, state.scrollParents.popper);
-        if (scroll) {
-            scrollParents.forEach(function(scrollParent) {
-                scrollParent.addEventListener("scroll", instance2.update, passive);
-            });
-        }
-        if (resize) {
-            window2.addEventListener("resize", instance2.update, passive);
-        }
-        return function() {
-            if (scroll) {
-                scrollParents.forEach(function(scrollParent) {
-                    scrollParent.removeEventListener("scroll", instance2.update, passive);
-                });
-            }
-            if (resize) {
-                window2.removeEventListener("resize", instance2.update, passive);
-            }
-        };
-    }
-    const eventListeners = {
-        name: "eventListeners",
-        enabled: true,
-        phase: "write",
-        fn: function fn2() {},
-        effect: effect$2,
-        data: {}
-    };
-
-    function getVariation(placement) {
-        return placement.split("-")[1];
-    }
-
-    function getMainAxisFromPlacement(placement) {
-        return ["top", "bottom"].indexOf(placement) >= 0 ? "x" : "y";
-    }
-
-    function computeOffsets(_ref2) {
-        var reference2 = _ref2.reference,
-            element2 = _ref2.element,
-            placement = _ref2.placement;
-        var basePlacement = placement ? getBasePlacement(placement) : null;
-        var variation = placement ? getVariation(placement) : null;
-        var commonX = reference2.x + reference2.width / 2 - element2.width / 2;
-        var commonY = reference2.y + reference2.height / 2 - element2.height / 2;
-        var offsets;
-        switch (basePlacement) {
-            case top$1:
-                offsets = {
-                    x: commonX,
-                    y: reference2.y - element2.height
-                };
-                break;
-            case bottom:
-                offsets = {
-                    x: commonX,
-                    y: reference2.y + reference2.height
-                };
-                break;
-            case right:
-                offsets = {
-                    x: reference2.x + reference2.width,
-                    y: commonY
-                };
-                break;
-            case left:
-                offsets = {
-                    x: reference2.x - element2.width,
-                    y: commonY
-                };
-                break;
-            default:
-                offsets = {
-                    x: reference2.x,
-                    y: reference2.y
-                };
-        }
-        var mainAxis = basePlacement ? getMainAxisFromPlacement(basePlacement) : null;
-        if (mainAxis != null) {
-            var len = mainAxis === "y" ? "height" : "width";
-            switch (variation) {
-                case start$1:
-                    offsets[mainAxis] = Math.floor(offsets[mainAxis]) - Math.floor(reference2[len] / 2 - element2[len] / 2);
-                    break;
-                case end:
-                    offsets[mainAxis] = Math.floor(offsets[mainAxis]) + Math.ceil(reference2[len] / 2 - element2[len] / 2);
-                    break;
-            }
-        }
-        return offsets;
-    }
-
-    function popperOffsets(_ref2) {
-        var state = _ref2.state,
-            name2 = _ref2.name;
-        state.modifiersData[name2] = computeOffsets({
-            reference: state.rects.reference,
-            element: state.rects.popper,
-            strategy: "absolute",
-            placement: state.placement
-        });
-    }
-    const popperOffsets$1 = {
-        name: "popperOffsets",
-        enabled: true,
-        phase: "read",
-        fn: popperOffsets,
-        data: {}
-    };
-    var unsetSides = {
-        top: "auto",
-        right: "auto",
-        bottom: "auto",
-        left: "auto"
-    };
-
-    function roundOffsets(_ref2) {
-        var x2 = _ref2.x,
-            y2 = _ref2.y;
-        var win = window;
-        var dpr = win.devicePixelRatio || 1;
-        return {
-            x: Math.round(x2 * dpr) / dpr || 0,
-            y: Math.round(y2 * dpr) / dpr || 0
-        };
-    }
-
-    function mapToStyles(_ref2) {
-        var _Object$assign2;
-        var popper2 = _ref2.popper,
-            popperRect = _ref2.popperRect,
-            placement = _ref2.placement,
-            offsets = _ref2.offsets,
-            position2 = _ref2.position,
-            gpuAcceleration = _ref2.gpuAcceleration,
-            adaptive = _ref2.adaptive;
-        var _roundOffsets = roundOffsets(offsets),
-            x2 = _roundOffsets.x,
-            y2 = _roundOffsets.y;
-        var hasX = offsets.hasOwnProperty("x");
-        var hasY = offsets.hasOwnProperty("y");
-        var sideX = left;
-        var sideY = top$1;
-        var win = window;
-        if (adaptive) {
-            var offsetParent = getOffsetParent$1(popper2);
-            if (offsetParent === getWindow$1(popper2)) {
-                offsetParent = getDocumentElement$1(popper2);
-            }
-            if (placement === top$1) {
-                sideY = bottom;
-                y2 -= offsetParent.clientHeight - popperRect.height;
-                y2 *= gpuAcceleration ? 1 : -1;
-            }
-            if (placement === left) {
-                sideX = right;
-                x2 -= offsetParent.clientWidth - popperRect.width;
-                x2 *= gpuAcceleration ? 1 : -1;
-            }
-        }
-        var commonStyles = Object.assign({
-            position: position2
-        }, adaptive && unsetSides);
-        if (gpuAcceleration) {
-            var _Object$assign;
-            return Object.assign({}, commonStyles, (_Object$assign = {}, _Object$assign[sideY] = hasY ? "0" : "", _Object$assign[sideX] = hasX ? "0" : "", _Object$assign.transform = (win.devicePixelRatio || 1) < 2 ? "translate(" + x2 + "px, " + y2 + "px)" : "translate3d(" + x2 + "px, " + y2 + "px, 0)", _Object$assign));
-        }
-        return Object.assign({}, commonStyles, (_Object$assign2 = {}, _Object$assign2[sideY] = hasY ? y2 + "px" : "", _Object$assign2[sideX] = hasX ? x2 + "px" : "", _Object$assign2.transform = "", _Object$assign2));
-    }
-
-    function computeStyles(_ref3) {
-        var state = _ref3.state,
-            options = _ref3.options;
-        var _options$gpuAccelerat = options.gpuAcceleration,
-            gpuAcceleration = _options$gpuAccelerat === void 0 ? true : _options$gpuAccelerat,
-            _options$adaptive = options.adaptive,
-            adaptive = _options$adaptive === void 0 ? true : _options$adaptive;
-        var commonStyles = {
-            placement: getBasePlacement(state.placement),
-            popper: state.elements.popper,
-            popperRect: state.rects.popper,
-            gpuAcceleration
-        };
-        if (state.modifiersData.popperOffsets != null) {
-            state.styles.popper = Object.assign({}, state.styles.popper, {}, mapToStyles(Object.assign({}, commonStyles, {
-                offsets: state.modifiersData.popperOffsets,
-                position: state.options.strategy,
-                adaptive
-            })));
-        }
-        if (state.modifiersData.arrow != null) {
-            state.styles.arrow = Object.assign({}, state.styles.arrow, {}, mapToStyles(Object.assign({}, commonStyles, {
-                offsets: state.modifiersData.arrow,
-                position: "absolute",
-                adaptive: false
-            })));
-        }
-        state.attributes.popper = Object.assign({}, state.attributes.popper, {
-            "data-popper-placement": state.placement
-        });
-    }
-    const computeStyles$1 = {
-        name: "computeStyles",
-        enabled: true,
-        phase: "beforeWrite",
-        fn: computeStyles,
-        data: {}
-    };
-
-    function applyStyles(_ref2) {
-        var state = _ref2.state;
-        Object.keys(state.elements).forEach(function(name2) {
-            var style2 = state.styles[name2] || {};
-            var attributes2 = state.attributes[name2] || {};
-            var element2 = state.elements[name2];
-            if (!isHTMLElement$1(element2) || !getNodeName$1(element2)) {
-                return;
-            }
-            Object.assign(element2.style, style2);
-            Object.keys(attributes2).forEach(function(name3) {
-                var value = attributes2[name3];
-                if (value === false) {
-                    element2.removeAttribute(name3);
-                } else {
-                    element2.setAttribute(name3, value === true ? "" : value);
-                }
-            });
-        });
-    }
-
-    function effect$1(_ref2) {
-        var state = _ref2.state;
-        var initialStyles = {
-            popper: {
-                position: state.options.strategy,
-                left: "0",
-                top: "0",
-                margin: "0"
-            },
-            arrow: {
-                position: "absolute"
-            },
-            reference: {}
-        };
-        Object.assign(state.elements.popper.style, initialStyles.popper);
-        if (state.elements.arrow) {
-            Object.assign(state.elements.arrow.style, initialStyles.arrow);
-        }
-        return function() {
-            Object.keys(state.elements).forEach(function(name2) {
-                var element2 = state.elements[name2];
-                var attributes2 = state.attributes[name2] || {};
-                var styleProperties = Object.keys(state.styles.hasOwnProperty(name2) ? state.styles[name2] : initialStyles[name2]);
-                var style2 = styleProperties.reduce(function(style3, property) {
-                    style3[property] = "";
-                    return style3;
-                }, {});
-                if (!isHTMLElement$1(element2) || !getNodeName$1(element2)) {
-                    return;
-                }
-                Object.assign(element2.style, style2);
-                Object.keys(attributes2).forEach(function(attribute) {
-                    element2.removeAttribute(attribute);
-                });
-            });
-        };
-    }
-    const applyStyles$1 = {
-        name: "applyStyles",
-        enabled: true,
-        phase: "write",
-        fn: applyStyles,
-        effect: effect$1,
-        requires: ["computeStyles"]
-    };
-
-    function distanceAndSkiddingToXY(placement, rects, offset2) {
-        var basePlacement = getBasePlacement(placement);
-        var invertDistance = [left, top$1].indexOf(basePlacement) >= 0 ? -1 : 1;
-        var _ref2 = typeof offset2 === "function" ? offset2(Object.assign({}, rects, {
-                placement
-            })) : offset2,
-            skidding = _ref2[0],
-            distance = _ref2[1];
-        skidding = skidding || 0;
-        distance = (distance || 0) * invertDistance;
-        return [left, right].indexOf(basePlacement) >= 0 ? {
-            x: distance,
-            y: skidding
-        } : {
-            x: skidding,
-            y: distance
-        };
-    }
-
-    function offset(_ref2) {
-        var state = _ref2.state,
-            options = _ref2.options,
-            name2 = _ref2.name;
-        var _options$offset = options.offset,
-            offset2 = _options$offset === void 0 ? [0, 0] : _options$offset;
-        var data2 = placements$1.reduce(function(acc, placement) {
-            acc[placement] = distanceAndSkiddingToXY(placement, state.rects, offset2);
-            return acc;
-        }, {});
-        var _data$state$placement = data2[state.placement],
-            x2 = _data$state$placement.x,
-            y2 = _data$state$placement.y;
-        if (state.modifiersData.popperOffsets != null) {
-            state.modifiersData.popperOffsets.x += x2;
-            state.modifiersData.popperOffsets.y += y2;
-        }
-        state.modifiersData[name2] = data2;
-    }
-    const offset$1 = {
-        name: "offset",
-        enabled: true,
-        phase: "main",
-        requires: ["popperOffsets"],
-        fn: offset
-    };
-    var hash$2 = {
-        left: "right",
-        right: "left",
-        bottom: "top",
-        top: "bottom"
-    };
-
-    function getOppositePlacement$1(placement) {
-        return placement.replace(/left|right|bottom|top/g, function(matched) {
-            return hash$2[matched];
-        });
-    }
-    var hash$1 = {
-        start: "end",
-        end: "start"
-    };
-
-    function getOppositeVariationPlacement(placement) {
-        return placement.replace(/start|end/g, function(matched) {
-            return hash$1[matched];
-        });
-    }
-
-    function getViewportRect$1(element2) {
-        var win = getWindow$1(element2);
-        var visualViewport = win.visualViewport;
-        var width = win.innerWidth;
-        var height = win.innerHeight;
-        if (visualViewport && /iPhone|iPod|iPad/.test(navigator.platform)) {
-            width = visualViewport.width;
-            height = visualViewport.height;
-        }
-        return {
-            width,
-            height,
-            x: 0,
-            y: 0
-        };
-    }
-
-    function getDocumentRect$1(element2) {
-        var win = getWindow$1(element2);
-        var winScroll = getWindowScroll(element2);
-        var documentRect = getCompositeRect(getDocumentElement$1(element2), win);
-        documentRect.height = Math.max(documentRect.height, win.innerHeight);
-        documentRect.width = Math.max(documentRect.width, win.innerWidth);
-        documentRect.x = -winScroll.scrollLeft;
-        documentRect.y = -winScroll.scrollTop;
-        return documentRect;
-    }
-
-    function toNumber$3(cssValue) {
-        return parseFloat(cssValue) || 0;
-    }
-
-    function getBorders(element2) {
-        var computedStyle = isHTMLElement$1(element2) ? getComputedStyle$2(element2) : {};
-        return {
-            top: toNumber$3(computedStyle.borderTopWidth),
-            right: toNumber$3(computedStyle.borderRightWidth),
-            bottom: toNumber$3(computedStyle.borderBottomWidth),
-            left: toNumber$3(computedStyle.borderLeftWidth)
-        };
-    }
-
-    function getDecorations(element2) {
-        var win = getWindow$1(element2);
-        var borders = getBorders(element2);
-        var isHTML = getNodeName$1(element2) === "html";
-        var winScrollBarX = getWindowScrollBarX$1(element2);
-        var x2 = element2.clientWidth + borders.right;
-        var y2 = element2.clientHeight + borders.bottom;
-        if (isHTML && win.innerHeight - element2.clientHeight > 50) {
-            y2 = win.innerHeight - borders.bottom;
-        }
-        return {
-            top: isHTML ? 0 : element2.clientTop,
-            right: element2.clientLeft > borders.left ? borders.right : isHTML ? win.innerWidth - x2 - winScrollBarX : element2.offsetWidth - x2,
-            bottom: isHTML ? win.innerHeight - y2 : element2.offsetHeight - y2,
-            left: isHTML ? winScrollBarX : element2.clientLeft
-        };
-    }
-
-    function contains$1(parent, child) {
-        var isShadow = Boolean(child.getRootNode && child.getRootNode().host);
-        if (parent.contains(child)) {
-            return true;
-        } else if (isShadow) {
-            var next2 = child;
-            do {
-                if (next2 && parent.isSameNode(next2)) {
-                    return true;
-                }
-                next2 = next2.parentNode || next2.host;
-            } while (next2);
-        }
-        return false;
-    }
-
-    function rectToClientRect$1(rect) {
-        return Object.assign({}, rect, {
-            left: rect.x,
-            top: rect.y,
-            right: rect.x + rect.width,
-            bottom: rect.y + rect.height
-        });
-    }
-
-    function getClientRectFromMixedType(element2, clippingParent) {
-        return clippingParent === viewport ? rectToClientRect$1(getViewportRect$1(element2)) : isHTMLElement$1(clippingParent) ? getBoundingClientRect$1(clippingParent) : rectToClientRect$1(getDocumentRect$1(getDocumentElement$1(element2)));
-    }
-
-    function getClippingParents(element2) {
-        var clippingParents2 = listScrollParents(element2);
-        var canEscapeClipping = ["absolute", "fixed"].indexOf(getComputedStyle$2(element2).position) >= 0;
-        var clipperElement = canEscapeClipping && isHTMLElement$1(element2) ? getOffsetParent$1(element2) : element2;
-        if (!isElement$2(clipperElement)) {
-            return [];
-        }
-        return clippingParents2.filter(function(clippingParent) {
-            return isElement$2(clippingParent) && contains$1(clippingParent, clipperElement);
-        });
-    }
-
-    function getClippingRect$1(element2, boundary, rootBoundary) {
-        var mainClippingParents = boundary === "clippingParents" ? getClippingParents(element2) : [].concat(boundary);
-        var clippingParents2 = [].concat(mainClippingParents, [rootBoundary]);
-        var firstClippingParent = clippingParents2[0];
-        var clippingRect = clippingParents2.reduce(function(accRect, clippingParent) {
-            var rect = getClientRectFromMixedType(element2, clippingParent);
-            var decorations2 = getDecorations(isHTMLElement$1(clippingParent) ? clippingParent : getDocumentElement$1(element2));
-            accRect.top = Math.max(rect.top + decorations2.top, accRect.top);
-            accRect.right = Math.min(rect.right - decorations2.right, accRect.right);
-            accRect.bottom = Math.min(rect.bottom - decorations2.bottom, accRect.bottom);
-            accRect.left = Math.max(rect.left + decorations2.left, accRect.left);
-            return accRect;
-        }, getClientRectFromMixedType(element2, firstClippingParent));
-        clippingRect.width = clippingRect.right - clippingRect.left;
-        clippingRect.height = clippingRect.bottom - clippingRect.top;
-        clippingRect.x = clippingRect.left;
-        clippingRect.y = clippingRect.top;
-        return clippingRect;
-    }
-
-    function getFreshSideObject() {
-        return {
-            top: 0,
-            right: 0,
-            bottom: 0,
-            left: 0
-        };
-    }
-
-    function mergePaddingObject(paddingObject) {
-        return Object.assign({}, getFreshSideObject(), {}, paddingObject);
-    }
-
-    function expandToHashMap(value, keys2) {
-        return keys2.reduce(function(hashMap, key) {
-            hashMap[key] = value;
-            return hashMap;
-        }, {});
-    }
-
-    function detectOverflow$1(state, options) {
-        if (options === void 0) {
-            options = {};
-        }
-        var _options = options,
-            _options$placement = _options.placement,
-            placement = _options$placement === void 0 ? state.placement : _options$placement,
-            _options$boundary = _options.boundary,
-            boundary = _options$boundary === void 0 ? clippingParents : _options$boundary,
-            _options$rootBoundary = _options.rootBoundary,
-            rootBoundary = _options$rootBoundary === void 0 ? viewport : _options$rootBoundary,
-            _options$elementConte = _options.elementContext,
-            elementContext = _options$elementConte === void 0 ? popper : _options$elementConte,
-            _options$altBoundary = _options.altBoundary,
-            altBoundary = _options$altBoundary === void 0 ? false : _options$altBoundary,
-            _options$padding = _options.padding,
-            padding = _options$padding === void 0 ? 0 : _options$padding;
-        var paddingObject = mergePaddingObject(typeof padding !== "number" ? padding : expandToHashMap(padding, basePlacements));
-        var altContext = elementContext === popper ? reference : popper;
-        var referenceElement = state.elements.reference;
-        var popperRect = state.rects.popper;
-        var element2 = state.elements[altBoundary ? altContext : elementContext];
-        var clippingClientRect = getClippingRect$1(isElement$2(element2) ? element2 : element2.contextElement || getDocumentElement$1(state.elements.popper), boundary, rootBoundary);
-        var referenceClientRect = getBoundingClientRect$1(referenceElement);
-        var popperOffsets2 = computeOffsets({
-            reference: referenceClientRect,
-            element: popperRect,
-            strategy: "absolute",
-            placement
-        });
-        var popperClientRect = rectToClientRect$1(Object.assign({}, popperRect, {}, popperOffsets2));
-        var elementClientRect = elementContext === popper ? popperClientRect : referenceClientRect;
-        var overflowOffsets = {
-            top: clippingClientRect.top - elementClientRect.top + paddingObject.top,
-            bottom: elementClientRect.bottom - clippingClientRect.bottom + paddingObject.bottom,
-            left: clippingClientRect.left - elementClientRect.left + paddingObject.left,
-            right: elementClientRect.right - clippingClientRect.right + paddingObject.right
-        };
-        var offsetData = state.modifiersData.offset;
-        if (elementContext === popper && offsetData) {
-            var offset2 = offsetData[placement];
-            Object.keys(overflowOffsets).forEach(function(key) {
-                var multiply = [right, bottom].indexOf(key) >= 0 ? 1 : -1;
-                var axis = [top$1, bottom].indexOf(key) >= 0 ? "y" : "x";
-                overflowOffsets[key] += offset2[axis] * multiply;
-            });
-        }
-        return overflowOffsets;
-    }
-
-    function computeAutoPlacement(state, options) {
-        if (options === void 0) {
-            options = {};
-        }
-        var _options = options,
-            placement = _options.placement,
-            boundary = _options.boundary,
-            rootBoundary = _options.rootBoundary,
-            padding = _options.padding,
-            flipVariations = _options.flipVariations,
-            _options$allowedAutoP = _options.allowedAutoPlacements,
-            allowedAutoPlacements = _options$allowedAutoP === void 0 ? placements$1 : _options$allowedAutoP;
-        var variation = getVariation(placement);
-        var placements2 = (variation ? flipVariations ? variationPlacements : variationPlacements.filter(function(placement2) {
-            return getVariation(placement2) === variation;
-        }) : basePlacements).filter(function(placement2) {
-            return allowedAutoPlacements.indexOf(placement2) >= 0;
-        });
-        var overflows = placements2.reduce(function(acc, placement2) {
-            acc[placement2] = detectOverflow$1(state, {
-                placement: placement2,
-                boundary,
-                rootBoundary,
-                padding
-            })[getBasePlacement(placement2)];
-            return acc;
-        }, {});
-        return Object.keys(overflows).sort(function(a2, b2) {
-            return overflows[a2] - overflows[b2];
-        });
-    }
-
-    function getExpandedFallbackPlacements(placement) {
-        if (getBasePlacement(placement) === auto) {
-            return [];
-        }
-        var oppositePlacement = getOppositePlacement$1(placement);
-        return [getOppositeVariationPlacement(placement), oppositePlacement, getOppositeVariationPlacement(oppositePlacement)];
-    }
-
-    function flip$2(_ref2) {
-        var state = _ref2.state,
-            options = _ref2.options,
-            name2 = _ref2.name;
-        if (state.modifiersData[name2]._skip) {
-            return;
-        }
-        var _options$mainAxis = options.mainAxis,
-            checkMainAxis = _options$mainAxis === void 0 ? true : _options$mainAxis,
-            _options$altAxis = options.altAxis,
-            checkAltAxis = _options$altAxis === void 0 ? true : _options$altAxis,
-            specifiedFallbackPlacements = options.fallbackPlacements,
-            padding = options.padding,
-            boundary = options.boundary,
-            rootBoundary = options.rootBoundary,
-            altBoundary = options.altBoundary,
-            _options$flipVariatio = options.flipVariations,
-            flipVariations = _options$flipVariatio === void 0 ? true : _options$flipVariatio,
-            allowedAutoPlacements = options.allowedAutoPlacements;
-        var preferredPlacement = state.options.placement;
-        var basePlacement = getBasePlacement(preferredPlacement);
-        var isBasePlacement = basePlacement === preferredPlacement;
-        var fallbackPlacements = specifiedFallbackPlacements || (isBasePlacement || !flipVariations ? [getOppositePlacement$1(preferredPlacement)] : getExpandedFallbackPlacements(preferredPlacement));
-        var placements2 = [preferredPlacement].concat(fallbackPlacements).reduce(function(acc, placement2) {
-            return acc.concat(getBasePlacement(placement2) === auto ? computeAutoPlacement(state, {
-                placement: placement2,
-                boundary,
-                rootBoundary,
-                padding,
-                flipVariations,
-                allowedAutoPlacements
-            }) : placement2);
-        }, []);
-        var referenceRect = state.rects.reference;
-        var popperRect = state.rects.popper;
-        var checksMap = /* @__PURE__ */ new Map();
-        var makeFallbackChecks = true;
-        var firstFittingPlacement = placements2[0];
-        for (var i2 = 0; i2 < placements2.length; i2++) {
-            var placement = placements2[i2];
-            var _basePlacement = getBasePlacement(placement);
-            var isStartVariation = getVariation(placement) === start$1;
-            var isVertical = [top$1, bottom].indexOf(_basePlacement) >= 0;
-            var len = isVertical ? "width" : "height";
-            var overflow = detectOverflow$1(state, {
-                placement,
-                boundary,
-                rootBoundary,
-                altBoundary,
-                padding
-            });
-            var mainVariationSide = isVertical ? isStartVariation ? right : left : isStartVariation ? bottom : top$1;
-            if (referenceRect[len] > popperRect[len]) {
-                mainVariationSide = getOppositePlacement$1(mainVariationSide);
-            }
-            var altVariationSide = getOppositePlacement$1(mainVariationSide);
-            var checks2 = [];
-            if (checkMainAxis) {
-                checks2.push(overflow[_basePlacement] <= 0);
-            }
-            if (checkAltAxis) {
-                checks2.push(overflow[mainVariationSide] <= 0, overflow[altVariationSide] <= 0);
-            }
-            if (checks2.every(function(check) {
-                    return check;
-                })) {
-                firstFittingPlacement = placement;
-                makeFallbackChecks = false;
-                break;
-            }
-            checksMap.set(placement, checks2);
-        }
-        if (makeFallbackChecks) {
-            var numberOfChecks = flipVariations ? 3 : 1;
-            var _loop = function _loop2(_i3) {
-                var fittingPlacement = placements2.find(function(placement2) {
-                    var checks3 = checksMap.get(placement2);
-                    if (checks3) {
-                        return checks3.slice(0, _i3).every(function(check) {
-                            return check;
-                        });
-                    }
-                });
-                if (fittingPlacement) {
-                    firstFittingPlacement = fittingPlacement;
-                    return "break";
-                }
-            };
-            for (var _i2 = numberOfChecks; _i2 > 0; _i2--) {
-                var _ret = _loop(_i2);
-                if (_ret === "break")
-                    break;
-            }
-        }
-        if (state.placement !== firstFittingPlacement) {
-            state.modifiersData[name2]._skip = true;
-            state.placement = firstFittingPlacement;
-            state.reset = true;
-        }
-    }
-    const flip$3 = {
-        name: "flip",
-        enabled: true,
-        phase: "main",
-        fn: flip$2,
-        requiresIfExists: ["offset"],
-        data: {
-            _skip: false
-        }
-    };
-
-    function getAltAxis(axis) {
-        return axis === "x" ? "y" : "x";
-    }
-
-    function within(min2, value, max2) {
-        return Math.max(min2, Math.min(value, max2));
-    }
-
-    function preventOverflow(_ref2) {
-        var state = _ref2.state,
-            options = _ref2.options,
-            name2 = _ref2.name;
-        var _options$mainAxis = options.mainAxis,
-            checkMainAxis = _options$mainAxis === void 0 ? true : _options$mainAxis,
-            _options$altAxis = options.altAxis,
-            checkAltAxis = _options$altAxis === void 0 ? false : _options$altAxis,
-            boundary = options.boundary,
-            rootBoundary = options.rootBoundary,
-            altBoundary = options.altBoundary,
-            padding = options.padding,
-            _options$tether = options.tether,
-            tether = _options$tether === void 0 ? true : _options$tether,
-            _options$tetherOffset = options.tetherOffset,
-            tetherOffset = _options$tetherOffset === void 0 ? 0 : _options$tetherOffset;
-        var overflow = detectOverflow$1(state, {
-            boundary,
-            rootBoundary,
-            padding,
-            altBoundary
-        });
-        var basePlacement = getBasePlacement(state.placement);
-        var variation = getVariation(state.placement);
-        var isBasePlacement = !variation;
-        var mainAxis = getMainAxisFromPlacement(basePlacement);
-        var altAxis = getAltAxis(mainAxis);
-        var popperOffsets2 = state.modifiersData.popperOffsets;
-        var referenceRect = state.rects.reference;
-        var popperRect = state.rects.popper;
-        var tetherOffsetValue = typeof tetherOffset === "function" ? tetherOffset(Object.assign({}, state.rects, {
-            placement: state.placement
-        })) : tetherOffset;
-        var data2 = {
-            x: 0,
-            y: 0
-        };
-        if (!popperOffsets2) {
-            return;
-        }
-        if (checkMainAxis) {
-            var mainSide = mainAxis === "y" ? top$1 : left;
-            var altSide = mainAxis === "y" ? bottom : right;
-            var len = mainAxis === "y" ? "height" : "width";
-            var offset2 = popperOffsets2[mainAxis];
-            var min2 = popperOffsets2[mainAxis] + overflow[mainSide];
-            var max2 = popperOffsets2[mainAxis] - overflow[altSide];
-            var additive = tether ? -popperRect[len] / 2 : 0;
-            var minLen = variation === start$1 ? referenceRect[len] : popperRect[len];
-            var maxLen = variation === start$1 ? -popperRect[len] : -referenceRect[len];
-            var arrowElement = state.elements.arrow;
-            var arrowRect = tether && arrowElement ? getLayoutRect(arrowElement) : {
-                width: 0,
-                height: 0
-            };
-            var arrowPaddingObject = state.modifiersData["arrow#persistent"] ? state.modifiersData["arrow#persistent"].padding : getFreshSideObject();
-            var arrowPaddingMin = arrowPaddingObject[mainSide];
-            var arrowPaddingMax = arrowPaddingObject[altSide];
-            var arrowLen = within(0, referenceRect[len], arrowRect[len]);
-            var minOffset = isBasePlacement ? referenceRect[len] / 2 - additive - arrowLen - arrowPaddingMin - tetherOffsetValue : minLen - arrowLen - arrowPaddingMin - tetherOffsetValue;
-            var maxOffset2 = isBasePlacement ? -referenceRect[len] / 2 + additive + arrowLen + arrowPaddingMax + tetherOffsetValue : maxLen + arrowLen + arrowPaddingMax + tetherOffsetValue;
-            var arrowOffsetParent = state.elements.arrow && getOffsetParent$1(state.elements.arrow);
-            var clientOffset = arrowOffsetParent ? mainAxis === "y" ? arrowOffsetParent.clientTop || 0 : arrowOffsetParent.clientLeft || 0 : 0;
-            var offsetModifierValue = state.modifiersData.offset ? state.modifiersData.offset[state.placement][mainAxis] : 0;
-            var tetherMin = popperOffsets2[mainAxis] + minOffset - offsetModifierValue - clientOffset;
-            var tetherMax = popperOffsets2[mainAxis] + maxOffset2 - offsetModifierValue;
-            var preventedOffset = within(tether ? Math.min(min2, tetherMin) : min2, offset2, tether ? Math.max(max2, tetherMax) : max2);
-            popperOffsets2[mainAxis] = preventedOffset;
-            data2[mainAxis] = preventedOffset - offset2;
-        }
-        if (checkAltAxis) {
-            var _mainSide = mainAxis === "x" ? top$1 : left;
-            var _altSide = mainAxis === "x" ? bottom : right;
-            var _offset = popperOffsets2[altAxis];
-            var _min = _offset + overflow[_mainSide];
-            var _max = _offset - overflow[_altSide];
-            var _preventedOffset = within(_min, _offset, _max);
-            popperOffsets2[altAxis] = _preventedOffset;
-            data2[altAxis] = _preventedOffset - _offset;
-        }
-        state.modifiersData[name2] = data2;
-    }
-    const preventOverflow$1 = {
-        name: "preventOverflow",
-        enabled: true,
-        phase: "main",
-        fn: preventOverflow,
-        requiresIfExists: ["offset"]
-    };
-
-    function arrow$1(_ref2) {
-        var _state$modifiersData$;
-        var state = _ref2.state,
-            name2 = _ref2.name;
-        var arrowElement = state.elements.arrow;
-        var popperOffsets2 = state.modifiersData.popperOffsets;
-        var basePlacement = getBasePlacement(state.placement);
-        var axis = getMainAxisFromPlacement(basePlacement);
-        var isVertical = [left, right].indexOf(basePlacement) >= 0;
-        var len = isVertical ? "height" : "width";
-        if (!arrowElement || !popperOffsets2) {
-            return;
-        }
-        var paddingObject = state.modifiersData[name2 + "#persistent"].padding;
-        var arrowRect = getLayoutRect(arrowElement);
-        var minProp = axis === "y" ? top$1 : left;
-        var maxProp = axis === "y" ? bottom : right;
-        var endDiff = state.rects.reference[len] + state.rects.reference[axis] - popperOffsets2[axis] - state.rects.popper[len];
-        var startDiff = popperOffsets2[axis] - state.rects.reference[axis];
-        var arrowOffsetParent = getOffsetParent$1(arrowElement);
-        var clientSize = arrowOffsetParent ? axis === "y" ? arrowOffsetParent.clientHeight || 0 : arrowOffsetParent.clientWidth || 0 : 0;
-        var centerToReference = endDiff / 2 - startDiff / 2;
-        var min2 = paddingObject[minProp];
-        var max2 = clientSize - arrowRect[len] - paddingObject[maxProp];
-        var center2 = clientSize / 2 - arrowRect[len] / 2 + centerToReference;
-        var offset2 = within(min2, center2, max2);
-        var axisProp = axis;
-        state.modifiersData[name2] = (_state$modifiersData$ = {}, _state$modifiersData$[axisProp] = offset2, _state$modifiersData$.centerOffset = offset2 - center2, _state$modifiersData$);
-    }
-
-    function effect(_ref2) {
-        var state = _ref2.state,
-            options = _ref2.options,
-            name2 = _ref2.name;
-        var _options$element = options.element,
-            arrowElement = _options$element === void 0 ? "[data-popper-arrow]" : _options$element,
-            _options$padding = options.padding,
-            padding = _options$padding === void 0 ? 0 : _options$padding;
-        if (arrowElement == null) {
-            return;
-        }
-        if (typeof arrowElement === "string") {
-            arrowElement = state.elements.popper.querySelector(arrowElement);
-            if (!arrowElement) {
-                return;
-            }
-        }
-        if (!contains$1(state.elements.popper, arrowElement)) {
-            return;
-        }
-        state.elements.arrow = arrowElement;
-        state.modifiersData[name2 + "#persistent"] = {
-            padding: mergePaddingObject(typeof padding !== "number" ? padding : expandToHashMap(padding, basePlacements))
-        };
-    }
-    const arrow$2 = {
-        name: "arrow",
-        enabled: true,
-        phase: "main",
-        fn: arrow$1,
-        effect,
-        requires: ["popperOffsets"],
-        requiresIfExists: ["preventOverflow"]
-    };
-
-    function getSideOffsets$1(overflow, rect, preventedOffsets) {
-        if (preventedOffsets === void 0) {
-            preventedOffsets = {
-                x: 0,
-                y: 0
-            };
-        }
-        return {
-            top: overflow.top - rect.height - preventedOffsets.y,
-            right: overflow.right - rect.width + preventedOffsets.x,
-            bottom: overflow.bottom - rect.height + preventedOffsets.y,
-            left: overflow.left - rect.width - preventedOffsets.x
-        };
-    }
-
-    function isAnySideFullyClipped$1(overflow) {
-        return [top$1, right, bottom, left].some(function(side) {
-            return overflow[side] >= 0;
-        });
-    }
-
-    function hide$1(_ref2) {
-        var state = _ref2.state,
-            name2 = _ref2.name;
-        var referenceRect = state.rects.reference;
-        var popperRect = state.rects.popper;
-        var preventedOffsets = state.modifiersData.preventOverflow;
-        var referenceOverflow = detectOverflow$1(state, {
-            elementContext: "reference"
-        });
-        var popperAltOverflow = detectOverflow$1(state, {
-            altBoundary: true
-        });
-        var referenceClippingOffsets = getSideOffsets$1(referenceOverflow, referenceRect);
-        var popperEscapeOffsets = getSideOffsets$1(popperAltOverflow, popperRect, preventedOffsets);
-        var isReferenceHidden = isAnySideFullyClipped$1(referenceClippingOffsets);
-        var hasPopperEscaped = isAnySideFullyClipped$1(popperEscapeOffsets);
-        state.modifiersData[name2] = {
-            referenceClippingOffsets,
-            popperEscapeOffsets,
-            isReferenceHidden,
-            hasPopperEscaped
-        };
-        state.attributes.popper = Object.assign({}, state.attributes.popper, {
-            "data-popper-reference-hidden": isReferenceHidden,
-            "data-popper-escaped": hasPopperEscaped
-        });
-    }
-    const hide$2 = {
-        name: "hide",
-        enabled: true,
-        phase: "main",
-        requiresIfExists: ["preventOverflow"],
-        fn: hide$1
-    };
-    var defaultModifiers = [eventListeners, popperOffsets$1, computeStyles$1, applyStyles$1, offset$1, flip$3, preventOverflow$1, arrow$2, hide$2];
-    var createPopper = /* @__PURE__ */ popperGenerator({
-        defaultModifiers
-    });
-    var hasElementType = typeof Element !== "undefined";
-    var hasMap$1 = typeof Map === "function";
-    var hasSet$1 = typeof Set === "function";
-    var hasArrayBuffer = typeof ArrayBuffer === "function" && !!ArrayBuffer.isView;
-
-    function equal$1(a2, b2) {
-        if (a2 === b2)
-            return true;
-        if (a2 && b2 && typeof a2 == "object" && typeof b2 == "object") {
-            if (a2.constructor !== b2.constructor)
-                return false;
-            var length, i2, keys2;
-            if (Array.isArray(a2)) {
-                length = a2.length;
-                if (length != b2.length)
-                    return false;
-                for (i2 = length; i2-- !== 0;)
-                    if (!equal$1(a2[i2], b2[i2]))
-                        return false;
-                return true;
-            }
-            var it2;
-            if (hasMap$1 && a2 instanceof Map && b2 instanceof Map) {
-                if (a2.size !== b2.size)
-                    return false;
-                it2 = a2.entries();
-                while (!(i2 = it2.next()).done)
-                    if (!b2.has(i2.value[0]))
-                        return false;
-                it2 = a2.entries();
-                while (!(i2 = it2.next()).done)
-                    if (!equal$1(i2.value[1], b2.get(i2.value[0])))
-                        return false;
-                return true;
-            }
-            if (hasSet$1 && a2 instanceof Set && b2 instanceof Set) {
-                if (a2.size !== b2.size)
-                    return false;
-                it2 = a2.entries();
-                while (!(i2 = it2.next()).done)
-                    if (!b2.has(i2.value[0]))
-                        return false;
-                return true;
-            }
-            if (hasArrayBuffer && ArrayBuffer.isView(a2) && ArrayBuffer.isView(b2)) {
-                length = a2.length;
-                if (length != b2.length)
-                    return false;
-                for (i2 = length; i2-- !== 0;)
-                    if (a2[i2] !== b2[i2])
-                        return false;
-                return true;
-            }
-            if (a2.constructor === RegExp)
-                return a2.source === b2.source && a2.flags === b2.flags;
-            if (a2.valueOf !== Object.prototype.valueOf && typeof a2.valueOf === "function" && typeof b2.valueOf === "function")
-                return a2.valueOf() === b2.valueOf();
-            if (a2.toString !== Object.prototype.toString && typeof a2.toString === "function" && typeof b2.toString === "function")
-                return a2.toString() === b2.toString();
-            keys2 = Object.keys(a2);
-            length = keys2.length;
-            if (length !== Object.keys(b2).length)
-                return false;
-            for (i2 = length; i2-- !== 0;)
-                if (!Object.prototype.hasOwnProperty.call(b2, keys2[i2]))
-                    return false;
-            if (hasElementType && a2 instanceof Element)
-                return false;
-            for (i2 = length; i2-- !== 0;) {
-                if ((keys2[i2] === "_owner" || keys2[i2] === "__v" || keys2[i2] === "__o") && a2.$$typeof) {
-                    continue;
-                }
-                if (!equal$1(a2[keys2[i2]], b2[keys2[i2]]))
-                    return false;
-            }
-            return true;
-        }
-        return a2 !== a2 && b2 !== b2;
-    }
-    var reactFastCompare = function isEqual2(a2, b2) {
-        try {
-            return equal$1(a2, b2);
-        } catch (error2) {
-            if ((error2.message || "").match(/stack|recursion/i)) {
-                console.warn("react-fast-compare cannot handle circular refs");
-                return false;
-            }
-            throw error2;
-        }
-    };
-    var EMPTY_MODIFIERS$2 = [];
-    var usePopper$1 = function usePopper2(referenceElement, popperElement, options) {
-        if (options === void 0) {
-            options = {};
-        }
-        var prevOptions = React__namespace.useRef(null);
-        var optionsWithDefaults = {
-            onFirstUpdate: options.onFirstUpdate,
-            placement: options.placement || "bottom",
-            strategy: options.strategy || "absolute",
-            modifiers: options.modifiers || EMPTY_MODIFIERS$2
-        };
-        var _React$useState = React__namespace.useState({
-                styles: {
-                    popper: {
-                        position: optionsWithDefaults.strategy,
-                        left: "0",
-                        top: "0"
-                    },
-                    arrow: {
-                        position: "absolute"
-                    }
-                },
-                attributes: {}
-            }),
-            state = _React$useState[0],
-            setState = _React$useState[1];
-        var updateStateModifier = React__namespace.useMemo(function() {
-            return {
-                name: "updateState",
-                enabled: true,
-                phase: "write",
-                fn: function fn2(_ref2) {
-                    var state2 = _ref2.state;
-                    var elements = Object.keys(state2.elements);
-                    ReactDOM__namespace.flushSync(function() {
-                        setState({
-                            styles: fromEntries$1(elements.map(function(element2) {
-                                return [element2, state2.styles[element2] || {}];
-                            })),
-                            attributes: fromEntries$1(elements.map(function(element2) {
-                                return [element2, state2.attributes[element2]];
-                            }))
-                        });
-                    });
-                },
-                requires: ["computeStyles"]
-            };
-        }, []);
-        var popperOptions = React__namespace.useMemo(function() {
-            var newOptions = {
-                onFirstUpdate: optionsWithDefaults.onFirstUpdate,
-                placement: optionsWithDefaults.placement,
-                strategy: optionsWithDefaults.strategy,
-                modifiers: [].concat(optionsWithDefaults.modifiers, [updateStateModifier, {
-                    name: "applyStyles",
-                    enabled: false
-                }])
-            };
-            if (reactFastCompare(prevOptions.current, newOptions)) {
-                return prevOptions.current || newOptions;
-            } else {
-                prevOptions.current = newOptions;
-                return newOptions;
-            }
-        }, [optionsWithDefaults.onFirstUpdate, optionsWithDefaults.placement, optionsWithDefaults.strategy, optionsWithDefaults.modifiers, updateStateModifier]);
-        var popperInstanceRef = React__namespace.useRef();
-        useIsomorphicLayoutEffect$2(function() {
-            if (popperInstanceRef.current) {
-                popperInstanceRef.current.setOptions(popperOptions);
-            }
-        }, [popperOptions]);
-        useIsomorphicLayoutEffect$2(function() {
-            if (referenceElement == null || popperElement == null) {
-                return;
-            }
-            var createPopper$12 = options.createPopper || createPopper;
-            var popperInstance = createPopper$12(referenceElement, popperElement, popperOptions);
-            popperInstanceRef.current = popperInstance;
-            return function() {
-                popperInstance.destroy();
-                popperInstanceRef.current = null;
-            };
-        }, [referenceElement, popperElement, options.createPopper]);
-        return {
-            state: popperInstanceRef.current ? popperInstanceRef.current.state : null,
-            styles: state.styles,
-            attributes: state.attributes,
-            update: popperInstanceRef.current ? popperInstanceRef.current.update : null,
-            forceUpdate: popperInstanceRef.current ? popperInstanceRef.current.forceUpdate : null
-        };
-    };
     const {
         stateChangeTypes: stateChangeTypes$3
     } = useCombobox;
     const Wrapper$a = styled__default.default.div`
     display: inline-flex;
 
     width: 100%;
@@ -40335,25 +41505,15 @@
     margin: 0;
     padding: 0 0.25rem;
 
     background-color: transparent !important;
 `;
 
     function ComboBox(props) {
-        var _a3, _b, _c, _d, _e2, _f, _g;
-        const referenceElement = React.useRef(null);
-        const popperElement = React.useRef(null);
-        const {
-            styles: styles2,
-            attributes: attributes2,
-            update: update2
-        } = usePopper$1(referenceElement.current, popperElement.current, {
-            modifiers: [sameWidthModifier],
-            placement: "bottom-start"
-        });
+        var _a3, _b, _c, _d, _e2, _f;
         const [inputValue, setInputValue] = React.useState((_d = (_b = (_a3 = props.initialValue) === null || _a3 === void 0 ? void 0 : _a3.label) !== null && _b !== void 0 ? _b : (_c = props.selectedItem) === null || _c === void 0 ? void 0 : _c.label) !== null && _d !== void 0 ? _d : "");
         const [pendingHighlight, setPendingHighlight] = React.useState(null);
         const filteredItems = props.items.filter((item) => {
             var _a4;
             return inputValue ? (_a4 = item.label) === null || _a4 === void 0 ? void 0 : _a4.toLowerCase().includes(inputValue === null || inputValue === void 0 ? void 0 : inputValue.toLowerCase()) : true;
         });
         const {
@@ -40415,56 +41575,68 @@
             }
         }, [isOpen, pendingHighlight, setHighlightedIndex]);
         React.useEffect(() => {
             if (props.selectedItem === null) {
                 setInputValue("");
             }
         }, [props.selectedItem]);
-        React.useEffect(() => {
-            if (isOpen && update2) {
-                update2();
-            }
-        }, [isOpen, update2]);
+        const {
+            refs,
+            floatingStyles,
+            context: context2
+        } = useFloating({
+            open: isOpen,
+            middleware: [flip$2(), shift$1(), offset$2({
+                crossAxis: 1
+            }), matchWidthToReference(2)],
+            whileElementsMounted: isOpen ? autoUpdate : void 0
+        });
+        const role = useRole(context2, {
+            role: "combobox"
+        });
+        const {
+            getReferenceProps,
+            getFloatingProps
+        } = useInteractions([role]);
         const menuProps = getMenuProps();
         const setMenuRef = menuProps.ref;
-        delete menuProps.ref;
-        const setMenuReference = (value) => {
-            setMenuRef(value);
-            popperElement.current = value;
-        };
+        const setFloatingRef = refs.setFloating;
+        const mergedRefs = React.useCallback((node2) => {
+            setFloatingRef(node2);
+            setMenuRef(node2);
+        }, [setFloatingRef, setMenuRef]);
         return jsxRuntime.exports.jsx(Tooltip$1, {
             content: props.errorMsg,
             disabled: !props.errorMsg,
             styling: "error",
             children: jsxRuntime.exports.jsxs(Wrapper$a, {
                 className: props.className,
                 isDisabled: props.disabled,
                 isErrored: !!props.errorMsg,
                 isOpen,
                 style: props.style,
                 children: [jsxRuntime.exports.jsxs(InputWrapper$4, {
                     disabled: props.disabled,
                     isOpen,
-                    ref: referenceElement,
+                    ref: refs.setReference,
                     children: [jsxRuntime.exports.jsx(Input$2, Object.assign({}, getInputProps({
                         disabled: props.disabled
-                    }), {
+                    }), getReferenceProps(), {
                         placeholder: (_f = selectedItem === null ? props.placeholder : selectedItem === null || selectedItem === void 0 ? void 0 : selectedItem.label) !== null && _f !== void 0 ? _f : props.placeholder,
                         size: props.size
                     })), jsxRuntime.exports.jsx(ChevronButton$1, Object.assign({}, getToggleButtonProps(), {
                         children: jsxRuntime.exports.jsx(Chevron$2, {
                             disabled: props.disabled,
                             isOpen
                         })
                     }))]
-                }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsxs(DropdownList$3, Object.assign({}, menuProps, attributes2.popper, {
+                }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsxs(DropdownList$3, Object.assign({}, menuProps, getFloatingProps(), {
+                    ref: mergedRefs,
                     isOpen,
-                    ref: setMenuReference,
-                    style: Object.assign(Object.assign({}, styles2.popper), {
-                        width: parseFloat((_g = styles2.popper) === null || _g === void 0 ? void 0 : _g.width) + 2,
+                    style: Object.assign(Object.assign({}, floatingStyles), {
                         zIndex: 9999
                     }),
                     children: [filteredItems.length > 0 && filteredItems.map((item, index2) => React.createElement(ListItem, Object.assign({}, getItemProps({
                         index: index2,
                         item
                     }), {
                         hovered: index2 === highlightedIndex,
@@ -42368,15 +43540,15 @@
         if (isNaN(date.getTime())) {
             return new Date(NaN);
         }
         date.setFullYear(year);
         return date;
     }
 
-    function min$2(dirtyDatesArray) {
+    function min$1(dirtyDatesArray) {
         requiredArgs(1, arguments);
         var datesArray;
         if (dirtyDatesArray && typeof dirtyDatesArray.forEach === "function") {
             datesArray = dirtyDatesArray;
         } else if (_typeof$5(dirtyDatesArray) === "object" && dirtyDatesArray !== null) {
             datesArray = Array.prototype.slice.call(dirtyDatesArray);
         } else {
@@ -42388,15 +43560,15 @@
             if (result === void 0 || result > currentDate || isNaN(currentDate.getDate())) {
                 result = currentDate;
             }
         });
         return result || new Date(NaN);
     }
 
-    function max$3(dirtyDatesArray) {
+    function max$2(dirtyDatesArray) {
         requiredArgs(1, arguments);
         var datesArray;
         if (dirtyDatesArray && typeof dirtyDatesArray.forEach === "function") {
             datesArray = dirtyDatesArray;
         } else if (_typeof$5(dirtyDatesArray) === "object" && dirtyDatesArray !== null) {
             datesArray = Array.prototype.slice.call(dirtyDatesArray);
         } else {
@@ -45407,14 +46579,104 @@
             var key = _ref2[0],
                 value = _ref2[1];
             acc[key] = value;
             return acc;
         }, {});
     };
     var useIsomorphicLayoutEffect$1 = typeof window !== "undefined" && window.document && window.document.createElement ? React__namespace.useLayoutEffect : React__namespace.useEffect;
+    var hasElementType = typeof Element !== "undefined";
+    var hasMap$1 = typeof Map === "function";
+    var hasSet$1 = typeof Set === "function";
+    var hasArrayBuffer = typeof ArrayBuffer === "function" && !!ArrayBuffer.isView;
+
+    function equal$1(a2, b2) {
+        if (a2 === b2)
+            return true;
+        if (a2 && b2 && typeof a2 == "object" && typeof b2 == "object") {
+            if (a2.constructor !== b2.constructor)
+                return false;
+            var length, i2, keys2;
+            if (Array.isArray(a2)) {
+                length = a2.length;
+                if (length != b2.length)
+                    return false;
+                for (i2 = length; i2-- !== 0;)
+                    if (!equal$1(a2[i2], b2[i2]))
+                        return false;
+                return true;
+            }
+            var it2;
+            if (hasMap$1 && a2 instanceof Map && b2 instanceof Map) {
+                if (a2.size !== b2.size)
+                    return false;
+                it2 = a2.entries();
+                while (!(i2 = it2.next()).done)
+                    if (!b2.has(i2.value[0]))
+                        return false;
+                it2 = a2.entries();
+                while (!(i2 = it2.next()).done)
+                    if (!equal$1(i2.value[1], b2.get(i2.value[0])))
+                        return false;
+                return true;
+            }
+            if (hasSet$1 && a2 instanceof Set && b2 instanceof Set) {
+                if (a2.size !== b2.size)
+                    return false;
+                it2 = a2.entries();
+                while (!(i2 = it2.next()).done)
+                    if (!b2.has(i2.value[0]))
+                        return false;
+                return true;
+            }
+            if (hasArrayBuffer && ArrayBuffer.isView(a2) && ArrayBuffer.isView(b2)) {
+                length = a2.length;
+                if (length != b2.length)
+                    return false;
+                for (i2 = length; i2-- !== 0;)
+                    if (a2[i2] !== b2[i2])
+                        return false;
+                return true;
+            }
+            if (a2.constructor === RegExp)
+                return a2.source === b2.source && a2.flags === b2.flags;
+            if (a2.valueOf !== Object.prototype.valueOf && typeof a2.valueOf === "function" && typeof b2.valueOf === "function")
+                return a2.valueOf() === b2.valueOf();
+            if (a2.toString !== Object.prototype.toString && typeof a2.toString === "function" && typeof b2.toString === "function")
+                return a2.toString() === b2.toString();
+            keys2 = Object.keys(a2);
+            length = keys2.length;
+            if (length !== Object.keys(b2).length)
+                return false;
+            for (i2 = length; i2-- !== 0;)
+                if (!Object.prototype.hasOwnProperty.call(b2, keys2[i2]))
+                    return false;
+            if (hasElementType && a2 instanceof Element)
+                return false;
+            for (i2 = length; i2-- !== 0;) {
+                if ((keys2[i2] === "_owner" || keys2[i2] === "__v" || keys2[i2] === "__o") && a2.$$typeof) {
+                    continue;
+                }
+                if (!equal$1(a2[keys2[i2]], b2[keys2[i2]]))
+                    return false;
+            }
+            return true;
+        }
+        return a2 !== a2 && b2 !== b2;
+    }
+    var reactFastCompare = function isEqual2(a2, b2) {
+        try {
+            return equal$1(a2, b2);
+        } catch (error2) {
+            if ((error2.message || "").match(/stack|recursion/i)) {
+                console.warn("react-fast-compare cannot handle circular refs");
+                return false;
+            }
+            throw error2;
+        }
+    };
     var EMPTY_MODIFIERS$1 = [];
     var usePopper = function usePopper2(referenceElement, popperElement, options) {
         if (options === void 0) {
             options = {};
         }
         var prevOptions = React__namespace.useRef(null);
         var optionsWithDefaults = {
@@ -45483,16 +46745,16 @@
                 popperInstanceRef.current.setOptions(popperOptions);
             }
         }, [popperOptions]);
         useIsomorphicLayoutEffect$1(function() {
             if (referenceElement == null || popperElement == null) {
                 return;
             }
-            var createPopper2 = options.createPopper || createPopper$1;
-            var popperInstance = createPopper2(referenceElement, popperElement, popperOptions);
+            var createPopper$1 = options.createPopper || createPopper;
+            var popperInstance = createPopper$1(referenceElement, popperElement, popperOptions);
             popperInstanceRef.current = popperInstance;
             return function() {
                 popperInstance.destroy();
                 popperInstanceRef.current = null;
             };
         }, [referenceElement, popperElement, options.createPopper]);
         return {
@@ -46173,29 +47435,29 @@
     function ut$1(e3) {
         var t2 = e3.minDate,
             r2 = e3.includeDates;
         if (r2 && t2) {
             var n2 = r2.filter(function(e4) {
                 return differenceInCalendarDays(e4, t2) >= 0;
             });
-            return min$2(n2);
+            return min$1(n2);
         }
-        return r2 ? min$2(r2) : t2;
+        return r2 ? min$1(r2) : t2;
     }
 
     function ht$2(e3) {
         var t2 = e3.maxDate,
             r2 = e3.includeDates;
         if (r2 && t2) {
             var n2 = r2.filter(function(e4) {
                 return differenceInCalendarDays(e4, t2) <= 0;
             });
-            return max$3(n2);
+            return max$2(n2);
         }
-        return r2 ? max$3(r2) : t2;
+        return r2 ? max$2(r2) : t2;
     }
 
     function mt$1() {
         for (var e3 = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [], t2 = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "react-datepicker__day--highlighted", r2 = /* @__PURE__ */ new Map(), o2 = 0, a2 = e3.length; o2 < a2; o2++) {
             var s2 = e3[o2];
             if (isDate$1(s2)) {
                 var i2 = Ee$1(s2, "MM.dd.yyyy"),
@@ -48806,25 +50068,15 @@
 
     background-color: ${(props) => props.theme.colors.grey1};
     border: none;
     outline: 0;
 `;
 
     function DatepickerSelect(props) {
-        var _a3, _b, _c;
-        const referenceElement = React.useRef(null);
-        const popperElement = React.useRef(null);
-        const {
-            styles: styles2,
-            attributes: attributes2,
-            update: update2
-        } = usePopper$1(referenceElement.current, popperElement.current, {
-            modifiers: [sameWidthModifier],
-            placement: props.placement || "bottom-start"
-        });
+        var _a3;
         const [pendingHighlight, setPendingHighlight] = React.useState(null);
         const {
             isOpen,
             selectedItem,
             getToggleButtonProps,
             getMenuProps,
             highlightedIndex,
@@ -48854,67 +50106,74 @@
         }));
         React.useEffect(() => {
             if (isOpen && pendingHighlight !== null) {
                 setHighlightedIndex(pendingHighlight);
                 setPendingHighlight(null);
             }
         }, [isOpen, pendingHighlight, setHighlightedIndex]);
-        React.useEffect(() => {
-            if (isOpen && update2) {
-                update2();
-            }
-        }, [isOpen, update2]);
-        const buttonProps = getToggleButtonProps({
-            disabled: props.disabled
-        });
-        const setButtonRef = buttonProps.ref;
-        delete buttonProps.ref;
-        const setButtonReference = (value) => {
-            setButtonRef(value);
-            referenceElement.current = value;
-        };
+        const {
+            refs,
+            floatingStyles,
+            context: context2
+        } = useFloating({
+            open: isOpen,
+            placement: props.placement || "bottom-start",
+            middleware: [offset$2(8), flip$2(), shift$1()],
+            whileElementsMounted: isOpen ? autoUpdate : void 0
+        });
+        const role = useRole(context2, {
+            role: "listbox"
+        });
+        const {
+            getReferenceProps,
+            getFloatingProps
+        } = useInteractions([role]);
         const menuProps = getMenuProps();
         const setMenuRef = menuProps.ref;
-        delete menuProps.ref;
-        const setMenuReference = (value) => {
-            var _a4;
-            setMenuRef(value);
-            popperElement.current = value;
-            (_a4 = props.dropdownRef) === null || _a4 === void 0 ? void 0 : _a4.call(props, value);
-        };
+        const setFloatingRef = refs.setFloating;
+        const {
+            dropdownRef
+        } = props;
+        const mergedRefs = React__namespace.useCallback((node2) => {
+            setFloatingRef(node2);
+            setMenuRef(node2);
+            dropdownRef === null || dropdownRef === void 0 ? void 0 : dropdownRef(node2);
+        }, [setFloatingRef, setMenuRef, dropdownRef]);
         return jsxRuntime.exports.jsx(Tooltip$1, {
             content: props.errorMsg,
             disabled: !props.errorMsg,
             styling: "error",
             children: jsxRuntime.exports.jsxs(Wrapper$9, {
                 className: props.className,
                 isDisabled: props.disabled,
                 isErrored: !!props.errorMsg,
                 onClick: props.onClick,
                 style: props.style,
                 children: [jsxRuntime.exports.jsxs(SelectButtonPrimary, Object.assign({
                     disabled: props.disabled
-                }, buttonProps, {
-                    ref: setButtonReference,
+                }, getToggleButtonProps({
+                    disabled: props.disabled
+                }), {
+                    ref: refs.setReference
+                }, getReferenceProps(), {
                     type: "button",
                     children: [jsxRuntime.exports.jsx(SelectedItem$1, {
                         size: props.size,
                         children: selectedItem ? selectedItem.label : "Select"
                     }), jsxRuntime.exports.jsx(Chevron$2, {
                         disabled: props.disabled,
                         isOpen
                     })]
-                })), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(DropdownList$2, Object.assign({}, menuProps, attributes2.popper, {
-                    className: `${(_a3 = menuProps === null || menuProps === void 0 ? void 0 : menuProps.className) !== null && _a3 !== void 0 ? _a3 : ""} ${(_c = (_b = attributes2 === null || attributes2 === void 0 ? void 0 : attributes2.popper) === null || _b === void 0 ? void 0 : _b.className) !== null && _c !== void 0 ? _c : ""} ${props.itemClass}`,
+                })), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(DropdownList$2, Object.assign({}, menuProps, getFloatingProps(), {
+                    ref: mergedRefs,
+                    className: `${(_a3 = menuProps === null || menuProps === void 0 ? void 0 : menuProps.className) !== null && _a3 !== void 0 ? _a3 : ""} ${props.itemClass}`,
                     displacement: props.displacement,
                     isOpen,
                     maxItems: 7,
-                    ref: setMenuReference,
-                    style: Object.assign(Object.assign({}, styles2.popper), {
-                        marginTop: `0.8rem`,
+                    style: Object.assign(Object.assign({}, floatingStyles), {
                         width: "16.25rem",
                         zIndex: 9999
                     }),
                     children: props.items.map((item, index2) => {
                         const _a4 = getItemProps({
                                 index: index2,
                                 item
@@ -49713,3514 +50972,1272 @@
                     case 0:
                         if (!dt2.items)
                             return [3, 2];
                         items = fromList(dt2.items).filter(function(item) {
                             return item.kind === "file";
                         });
                         if (type2 !== "drop") {
-                            return [2, items];
-                        }
-                        return [4, Promise.all(items.map(toFilePromises))];
-                    case 1:
-                        files = _a3.sent();
-                        return [2, noIgnoredFiles(flatten$1(files))];
-                    case 2:
-                        return [2, noIgnoredFiles(fromList(dt2.files).map(function(file) {
-                            return toFileWithPath(file);
-                        }))];
-                }
-            });
-        });
-    }
-
-    function noIgnoredFiles(files) {
-        return files.filter(function(file) {
-            return FILES_TO_IGNORE.indexOf(file.name) === -1;
-        });
-    }
-
-    function fromList(items) {
-        var files = [];
-        for (var i2 = 0; i2 < items.length; i2++) {
-            var file = items[i2];
-            files.push(file);
-        }
-        return files;
-    }
-
-    function toFilePromises(item) {
-        if (typeof item.webkitGetAsEntry !== "function") {
-            return fromDataTransferItem(item);
-        }
-        var entry = item.webkitGetAsEntry();
-        if (entry && entry.isDirectory) {
-            return fromDirEntry(entry);
-        }
-        return fromDataTransferItem(item);
-    }
-
-    function flatten$1(items) {
-        return items.reduce(function(acc, files) {
-            return __spread(acc, Array.isArray(files) ? flatten$1(files) : [files]);
-        }, []);
-    }
-
-    function fromDataTransferItem(item) {
-        var file = item.getAsFile();
-        if (!file) {
-            return Promise.reject(item + " is not a File");
-        }
-        var fwp = toFileWithPath(file);
-        return Promise.resolve(fwp);
-    }
-
-    function fromEntry(entry) {
-        return __awaiter$2(this, void 0, void 0, function() {
-            return __generator(this, function(_a3) {
-                return [2, entry.isDirectory ? fromDirEntry(entry) : fromFileEntry(entry)];
-            });
-        });
-    }
-
-    function fromDirEntry(entry) {
-        var reader = entry.createReader();
-        return new Promise(function(resolve2, reject) {
-            var entries = [];
-
-            function readEntries() {
-                var _this = this;
-                reader.readEntries(function(batch) {
-                    return __awaiter$2(_this, void 0, void 0, function() {
-                        var files, err_1, items;
-                        return __generator(this, function(_a3) {
-                            switch (_a3.label) {
-                                case 0:
-                                    if (!!batch.length)
-                                        return [3, 5];
-                                    _a3.label = 1;
-                                case 1:
-                                    _a3.trys.push([1, 3, , 4]);
-                                    return [4, Promise.all(entries)];
-                                case 2:
-                                    files = _a3.sent();
-                                    resolve2(files);
-                                    return [3, 4];
-                                case 3:
-                                    err_1 = _a3.sent();
-                                    reject(err_1);
-                                    return [3, 4];
-                                case 4:
-                                    return [3, 6];
-                                case 5:
-                                    items = Promise.all(batch.map(fromEntry));
-                                    entries.push(items);
-                                    readEntries();
-                                    _a3.label = 6;
-                                case 6:
-                                    return [2];
-                            }
-                        });
-                    });
-                }, function(err) {
-                    reject(err);
-                });
-            }
-            readEntries();
-        });
-    }
-
-    function fromFileEntry(entry) {
-        return __awaiter$2(this, void 0, void 0, function() {
-            return __generator(this, function(_a3) {
-                return [2, new Promise(function(resolve2, reject) {
-                    entry.file(function(file) {
-                        var fwp = toFileWithPath(file, entry.fullPath);
-                        resolve2(fwp);
-                    }, function(err) {
-                        reject(err);
-                    });
-                })];
-            });
-        });
-    }
-    var _default$1 = function(file, acceptedFiles) {
-        if (file && acceptedFiles) {
-            var acceptedFilesArray = Array.isArray(acceptedFiles) ? acceptedFiles : acceptedFiles.split(",");
-            var fileName = file.name || "";
-            var mimeType = (file.type || "").toLowerCase();
-            var baseMimeType = mimeType.replace(/\/.*$/, "");
-            return acceptedFilesArray.some(function(type2) {
-                var validType = type2.trim().toLowerCase();
-                if (validType.charAt(0) === ".") {
-                    return fileName.toLowerCase().endsWith(validType);
-                } else if (validType.endsWith("/*")) {
-                    return baseMimeType === validType.replace(/\/.*$/, "");
-                }
-                return mimeType === validType;
-            });
-        }
-        return true;
-    };
-
-    function _slicedToArray$9(arr, i2) {
-        return _arrayWithHoles$9(arr) || _iterableToArrayLimit$9(arr, i2) || _nonIterableRest$9();
-    }
-
-    function _nonIterableRest$9() {
-        throw new TypeError("Invalid attempt to destructure non-iterable instance");
-    }
-
-    function _iterableToArrayLimit$9(arr, i2) {
-        if (!(Symbol.iterator in Object(arr) || Object.prototype.toString.call(arr) === "[object Arguments]")) {
-            return;
-        }
-        var _arr = [];
-        var _n2 = true;
-        var _d = false;
-        var _e2 = void 0;
-        try {
-            for (var _i2 = arr[Symbol.iterator](), _s; !(_n2 = (_s = _i2.next()).done); _n2 = true) {
-                _arr.push(_s.value);
-                if (i2 && _arr.length === i2)
-                    break;
-            }
-        } catch (err) {
-            _d = true;
-            _e2 = err;
-        } finally {
-            try {
-                if (!_n2 && _i2["return"] != null)
-                    _i2["return"]();
-            } finally {
-                if (_d)
-                    throw _e2;
-            }
-        }
-        return _arr;
-    }
-
-    function _arrayWithHoles$9(arr) {
-        if (Array.isArray(arr))
-            return arr;
-    }
-    var FILE_INVALID_TYPE = "file-invalid-type";
-    var FILE_TOO_LARGE = "file-too-large";
-    var FILE_TOO_SMALL = "file-too-small";
-    var TOO_MANY_FILES = "too-many-files";
-    var getInvalidTypeRejectionErr = function getInvalidTypeRejectionErr2(accept) {
-        accept = Array.isArray(accept) && accept.length === 1 ? accept[0] : accept;
-        var messageSuffix = Array.isArray(accept) ? "one of ".concat(accept.join(", ")) : accept;
-        return {
-            code: FILE_INVALID_TYPE,
-            message: "File type must be ".concat(messageSuffix)
-        };
-    };
-    var getTooLargeRejectionErr = function getTooLargeRejectionErr2(maxSize) {
-        return {
-            code: FILE_TOO_LARGE,
-            message: "File is larger than ".concat(maxSize, " bytes")
-        };
-    };
-    var getTooSmallRejectionErr = function getTooSmallRejectionErr2(minSize) {
-        return {
-            code: FILE_TOO_SMALL,
-            message: "File is smaller than ".concat(minSize, " bytes")
-        };
-    };
-    var TOO_MANY_FILES_REJECTION = {
-        code: TOO_MANY_FILES,
-        message: "Too many files"
-    };
-
-    function fileAccepted(file, accept) {
-        var isAcceptable = file.type === "application/x-moz-file" || _default$1(file, accept);
-        return [isAcceptable, isAcceptable ? null : getInvalidTypeRejectionErr(accept)];
-    }
-
-    function fileMatchSize(file, minSize, maxSize) {
-        if (isDefined(file.size)) {
-            if (isDefined(minSize) && isDefined(maxSize)) {
-                if (file.size > maxSize)
-                    return [false, getTooLargeRejectionErr(maxSize)];
-                if (file.size < minSize)
-                    return [false, getTooSmallRejectionErr(minSize)];
-            } else if (isDefined(minSize) && file.size < minSize)
-                return [false, getTooSmallRejectionErr(minSize)];
-            else if (isDefined(maxSize) && file.size > maxSize)
-                return [false, getTooLargeRejectionErr(maxSize)];
-        }
-        return [true, null];
-    }
-
-    function isDefined(value) {
-        return value !== void 0 && value !== null;
-    }
-
-    function allFilesAccepted(_ref2) {
-        var files = _ref2.files,
-            accept = _ref2.accept,
-            minSize = _ref2.minSize,
-            maxSize = _ref2.maxSize,
-            multiple = _ref2.multiple;
-        if (!multiple && files.length > 1) {
-            return false;
-        }
-        return files.every(function(file) {
-            var _fileAccepted = fileAccepted(file, accept),
-                _fileAccepted2 = _slicedToArray$9(_fileAccepted, 1),
-                accepted = _fileAccepted2[0];
-            var _fileMatchSize = fileMatchSize(file, minSize, maxSize),
-                _fileMatchSize2 = _slicedToArray$9(_fileMatchSize, 1),
-                sizeMatch = _fileMatchSize2[0];
-            return accepted && sizeMatch;
-        });
-    }
-
-    function isPropagationStopped(event2) {
-        if (typeof event2.isPropagationStopped === "function") {
-            return event2.isPropagationStopped();
-        } else if (typeof event2.cancelBubble !== "undefined") {
-            return event2.cancelBubble;
-        }
-        return false;
-    }
-
-    function isEvtWithFiles(event2) {
-        if (!event2.dataTransfer) {
-            return !!event2.target && !!event2.target.files;
-        }
-        return Array.prototype.some.call(event2.dataTransfer.types, function(type2) {
-            return type2 === "Files" || type2 === "application/x-moz-file";
-        });
-    }
-
-    function onDocumentDragOver(event2) {
-        event2.preventDefault();
-    }
-
-    function isIe(userAgent2) {
-        return userAgent2.indexOf("MSIE") !== -1 || userAgent2.indexOf("Trident/") !== -1;
-    }
-
-    function isEdge(userAgent2) {
-        return userAgent2.indexOf("Edge/") !== -1;
-    }
-
-    function isIeOrEdge() {
-        var userAgent2 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : window.navigator.userAgent;
-        return isIe(userAgent2) || isEdge(userAgent2);
-    }
-
-    function composeEventHandlers() {
-        for (var _len = arguments.length, fns = new Array(_len), _key = 0; _key < _len; _key++) {
-            fns[_key] = arguments[_key];
-        }
-        return function(event2) {
-            for (var _len2 = arguments.length, args = new Array(_len2 > 1 ? _len2 - 1 : 0), _key2 = 1; _key2 < _len2; _key2++) {
-                args[_key2 - 1] = arguments[_key2];
-            }
-            return fns.some(function(fn2) {
-                if (!isPropagationStopped(event2) && fn2) {
-                    fn2.apply(void 0, [event2].concat(args));
-                }
-                return isPropagationStopped(event2);
-            });
-        };
-    }
-
-    function _toConsumableArray$2(arr) {
-        return _arrayWithoutHoles$2(arr) || _iterableToArray$2(arr) || _nonIterableSpread$2();
-    }
-
-    function _nonIterableSpread$2() {
-        throw new TypeError("Invalid attempt to spread non-iterable instance");
-    }
-
-    function _iterableToArray$2(iter2) {
-        if (Symbol.iterator in Object(iter2) || Object.prototype.toString.call(iter2) === "[object Arguments]")
-            return Array.from(iter2);
-    }
-
-    function _arrayWithoutHoles$2(arr) {
-        if (Array.isArray(arr)) {
-            for (var i2 = 0, arr2 = new Array(arr.length); i2 < arr.length; i2++) {
-                arr2[i2] = arr[i2];
-            }
-            return arr2;
-        }
-    }
-
-    function _slicedToArray$8(arr, i2) {
-        return _arrayWithHoles$8(arr) || _iterableToArrayLimit$8(arr, i2) || _nonIterableRest$8();
-    }
-
-    function _nonIterableRest$8() {
-        throw new TypeError("Invalid attempt to destructure non-iterable instance");
-    }
-
-    function _iterableToArrayLimit$8(arr, i2) {
-        if (!(Symbol.iterator in Object(arr) || Object.prototype.toString.call(arr) === "[object Arguments]")) {
-            return;
-        }
-        var _arr = [];
-        var _n2 = true;
-        var _d = false;
-        var _e2 = void 0;
-        try {
-            for (var _i2 = arr[Symbol.iterator](), _s; !(_n2 = (_s = _i2.next()).done); _n2 = true) {
-                _arr.push(_s.value);
-                if (i2 && _arr.length === i2)
-                    break;
-            }
-        } catch (err) {
-            _d = true;
-            _e2 = err;
-        } finally {
-            try {
-                if (!_n2 && _i2["return"] != null)
-                    _i2["return"]();
-            } finally {
-                if (_d)
-                    throw _e2;
-            }
-        }
-        return _arr;
-    }
-
-    function _arrayWithHoles$8(arr) {
-        if (Array.isArray(arr))
-            return arr;
-    }
-
-    function ownKeys$6(object2, enumerableOnly) {
-        var keys2 = Object.keys(object2);
-        if (Object.getOwnPropertySymbols) {
-            var symbols = Object.getOwnPropertySymbols(object2);
-            if (enumerableOnly)
-                symbols = symbols.filter(function(sym) {
-                    return Object.getOwnPropertyDescriptor(object2, sym).enumerable;
-                });
-            keys2.push.apply(keys2, symbols);
-        }
-        return keys2;
-    }
-
-    function _objectSpread$5(target) {
-        for (var i2 = 1; i2 < arguments.length; i2++) {
-            var source = arguments[i2] != null ? arguments[i2] : {};
-            if (i2 % 2) {
-                ownKeys$6(source, true).forEach(function(key) {
-                    _defineProperty$n(target, key, source[key]);
-                });
-            } else if (Object.getOwnPropertyDescriptors) {
-                Object.defineProperties(target, Object.getOwnPropertyDescriptors(source));
-            } else {
-                ownKeys$6(source).forEach(function(key) {
-                    Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));
-                });
-            }
-        }
-        return target;
-    }
-
-    function _defineProperty$n(obj, key, value) {
-        if (key in obj) {
-            Object.defineProperty(obj, key, {
-                value,
-                enumerable: true,
-                configurable: true,
-                writable: true
-            });
-        } else {
-            obj[key] = value;
-        }
-        return obj;
-    }
-
-    function _objectWithoutProperties$1(source, excluded) {
-        if (source == null)
-            return {};
-        var target = _objectWithoutPropertiesLoose$2(source, excluded);
-        var key, i2;
-        if (Object.getOwnPropertySymbols) {
-            var sourceSymbolKeys = Object.getOwnPropertySymbols(source);
-            for (i2 = 0; i2 < sourceSymbolKeys.length; i2++) {
-                key = sourceSymbolKeys[i2];
-                if (excluded.indexOf(key) >= 0)
-                    continue;
-                if (!Object.prototype.propertyIsEnumerable.call(source, key))
-                    continue;
-                target[key] = source[key];
-            }
-        }
-        return target;
-    }
-
-    function _objectWithoutPropertiesLoose$2(source, excluded) {
-        if (source == null)
-            return {};
-        var target = {};
-        var sourceKeys = Object.keys(source);
-        var key, i2;
-        for (i2 = 0; i2 < sourceKeys.length; i2++) {
-            key = sourceKeys[i2];
-            if (excluded.indexOf(key) >= 0)
-                continue;
-            target[key] = source[key];
-        }
-        return target;
-    }
-    var Dropzone$1 = React.forwardRef(function(_ref2, ref2) {
-        var children2 = _ref2.children,
-            params = _objectWithoutProperties$1(_ref2, ["children"]);
-        var _useDropzone = useDropzone(params),
-            open = _useDropzone.open,
-            props = _objectWithoutProperties$1(_useDropzone, ["open"]);
-        React.useImperativeHandle(ref2, function() {
-            return {
-                open
-            };
-        }, [open]);
-        return React__default.default.createElement(React.Fragment, null, children2(_objectSpread$5({}, props, {
-            open
-        })));
-    });
-    Dropzone$1.displayName = "Dropzone";
-    Dropzone$1.propTypes = {
-        children: propTypes.exports.func,
-        accept: propTypes.exports.oneOfType([propTypes.exports.string, propTypes.exports.arrayOf(propTypes.exports.string)]),
-        multiple: propTypes.exports.bool,
-        preventDropOnDocument: propTypes.exports.bool,
-        noClick: propTypes.exports.bool,
-        noKeyboard: propTypes.exports.bool,
-        noDrag: propTypes.exports.bool,
-        noDragEventsBubbling: propTypes.exports.bool,
-        minSize: propTypes.exports.number,
-        maxSize: propTypes.exports.number,
-        disabled: propTypes.exports.bool,
-        getFilesFromEvent: propTypes.exports.func,
-        onFileDialogCancel: propTypes.exports.func,
-        onDragEnter: propTypes.exports.func,
-        onDragLeave: propTypes.exports.func,
-        onDragOver: propTypes.exports.func,
-        onDrop: propTypes.exports.func,
-        onDropAccepted: propTypes.exports.func,
-        onDropRejected: propTypes.exports.func
-    };
-    var initialState$2 = {
-        isFocused: false,
-        isFileDialogActive: false,
-        isDragActive: false,
-        isDragAccept: false,
-        isDragReject: false,
-        draggedFiles: [],
-        acceptedFiles: [],
-        fileRejections: []
-    };
-
-    function useDropzone() {
-        var _ref2 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
-            accept = _ref2.accept,
-            _ref2$disabled = _ref2.disabled,
-            disabled2 = _ref2$disabled === void 0 ? false : _ref2$disabled,
-            _ref2$getFilesFromEve = _ref2.getFilesFromEvent,
-            getFilesFromEvent = _ref2$getFilesFromEve === void 0 ? fromEvent : _ref2$getFilesFromEve,
-            _ref2$maxSize = _ref2.maxSize,
-            maxSize = _ref2$maxSize === void 0 ? Infinity : _ref2$maxSize,
-            _ref2$minSize = _ref2.minSize,
-            minSize = _ref2$minSize === void 0 ? 0 : _ref2$minSize,
-            _ref2$multiple = _ref2.multiple,
-            multiple = _ref2$multiple === void 0 ? true : _ref2$multiple,
-            onDragEnter = _ref2.onDragEnter,
-            onDragLeave = _ref2.onDragLeave,
-            onDragOver = _ref2.onDragOver,
-            onDrop = _ref2.onDrop,
-            onDropAccepted = _ref2.onDropAccepted,
-            onDropRejected = _ref2.onDropRejected,
-            onFileDialogCancel = _ref2.onFileDialogCancel,
-            _ref2$preventDropOnDo = _ref2.preventDropOnDocument,
-            preventDropOnDocument = _ref2$preventDropOnDo === void 0 ? true : _ref2$preventDropOnDo,
-            _ref2$noClick = _ref2.noClick,
-            noClick = _ref2$noClick === void 0 ? false : _ref2$noClick,
-            _ref2$noKeyboard = _ref2.noKeyboard,
-            noKeyboard = _ref2$noKeyboard === void 0 ? false : _ref2$noKeyboard,
-            _ref2$noDrag = _ref2.noDrag,
-            noDrag = _ref2$noDrag === void 0 ? false : _ref2$noDrag,
-            _ref2$noDragEventsBub = _ref2.noDragEventsBubbling,
-            noDragEventsBubbling = _ref2$noDragEventsBub === void 0 ? false : _ref2$noDragEventsBub;
-        var rootRef = React.useRef(null);
-        var inputRef = React.useRef(null);
-        var _useReducer = React.useReducer(reducer, initialState$2),
-            _useReducer2 = _slicedToArray$8(_useReducer, 2),
-            state = _useReducer2[0],
-            dispatch2 = _useReducer2[1];
-        var isFocused = state.isFocused,
-            isFileDialogActive = state.isFileDialogActive,
-            draggedFiles = state.draggedFiles;
-        var openFileDialog = React.useCallback(function() {
-            if (inputRef.current) {
-                dispatch2({
-                    type: "openDialog"
-                });
-                inputRef.current.value = null;
-                inputRef.current.click();
-            }
-        }, [dispatch2]);
-        var onWindowFocus = function onWindowFocus2() {
-            if (isFileDialogActive) {
-                setTimeout(function() {
-                    if (inputRef.current) {
-                        var files = inputRef.current.files;
-                        if (!files.length) {
-                            dispatch2({
-                                type: "closeDialog"
-                            });
-                            if (typeof onFileDialogCancel === "function") {
-                                onFileDialogCancel();
-                            }
-                        }
-                    }
-                }, 300);
-            }
-        };
-        React.useEffect(function() {
-            window.addEventListener("focus", onWindowFocus, false);
-            return function() {
-                window.removeEventListener("focus", onWindowFocus, false);
-            };
-        }, [inputRef, isFileDialogActive, onFileDialogCancel]);
-        var onKeyDownCb = React.useCallback(function(event2) {
-            if (!rootRef.current || !rootRef.current.isEqualNode(event2.target)) {
-                return;
-            }
-            if (event2.keyCode === 32 || event2.keyCode === 13) {
-                event2.preventDefault();
-                openFileDialog();
-            }
-        }, [rootRef, inputRef]);
-        var onFocusCb = React.useCallback(function() {
-            dispatch2({
-                type: "focus"
-            });
-        }, []);
-        var onBlurCb = React.useCallback(function() {
-            dispatch2({
-                type: "blur"
-            });
-        }, []);
-        var onClickCb = React.useCallback(function() {
-            if (noClick) {
-                return;
-            }
-            if (isIeOrEdge()) {
-                setTimeout(openFileDialog, 0);
-            } else {
-                openFileDialog();
-            }
-        }, [inputRef, noClick]);
-        var dragTargetsRef = React.useRef([]);
-        var onDocumentDrop = function onDocumentDrop2(event2) {
-            if (rootRef.current && rootRef.current.contains(event2.target)) {
-                return;
-            }
-            event2.preventDefault();
-            dragTargetsRef.current = [];
-        };
-        React.useEffect(function() {
-            if (preventDropOnDocument) {
-                document.addEventListener("dragover", onDocumentDragOver, false);
-                document.addEventListener("drop", onDocumentDrop, false);
-            }
-            return function() {
-                if (preventDropOnDocument) {
-                    document.removeEventListener("dragover", onDocumentDragOver);
-                    document.removeEventListener("drop", onDocumentDrop);
-                }
-            };
-        }, [rootRef, preventDropOnDocument]);
-        var onDragEnterCb = React.useCallback(function(event2) {
-            event2.preventDefault();
-            event2.persist();
-            stopPropagation(event2);
-            dragTargetsRef.current = [].concat(_toConsumableArray$2(dragTargetsRef.current), [event2.target]);
-            if (isEvtWithFiles(event2)) {
-                Promise.resolve(getFilesFromEvent(event2)).then(function(draggedFiles2) {
-                    if (isPropagationStopped(event2) && !noDragEventsBubbling) {
-                        return;
-                    }
-                    dispatch2({
-                        draggedFiles: draggedFiles2,
-                        isDragActive: true,
-                        type: "setDraggedFiles"
-                    });
-                    if (onDragEnter) {
-                        onDragEnter(event2);
-                    }
-                });
-            }
-        }, [getFilesFromEvent, onDragEnter, noDragEventsBubbling]);
-        var onDragOverCb = React.useCallback(function(event2) {
-            event2.preventDefault();
-            event2.persist();
-            stopPropagation(event2);
-            if (event2.dataTransfer) {
-                try {
-                    event2.dataTransfer.dropEffect = "copy";
-                } catch (_unused) {}
-            }
-            if (isEvtWithFiles(event2) && onDragOver) {
-                onDragOver(event2);
-            }
-            return false;
-        }, [onDragOver, noDragEventsBubbling]);
-        var onDragLeaveCb = React.useCallback(function(event2) {
-            event2.preventDefault();
-            event2.persist();
-            stopPropagation(event2);
-            var targets = dragTargetsRef.current.filter(function(target) {
-                return rootRef.current && rootRef.current.contains(target);
-            });
-            var targetIdx = targets.indexOf(event2.target);
-            if (targetIdx !== -1) {
-                targets.splice(targetIdx, 1);
-            }
-            dragTargetsRef.current = targets;
-            if (targets.length > 0) {
-                return;
-            }
-            dispatch2({
-                isDragActive: false,
-                type: "setDraggedFiles",
-                draggedFiles: []
-            });
-            if (isEvtWithFiles(event2) && onDragLeave) {
-                onDragLeave(event2);
-            }
-        }, [rootRef, onDragLeave, noDragEventsBubbling]);
-        var onDropCb = React.useCallback(function(event2) {
-            event2.preventDefault();
-            event2.persist();
-            stopPropagation(event2);
-            dragTargetsRef.current = [];
-            if (isEvtWithFiles(event2)) {
-                Promise.resolve(getFilesFromEvent(event2)).then(function(files) {
-                    if (isPropagationStopped(event2) && !noDragEventsBubbling) {
-                        return;
-                    }
-                    var acceptedFiles = [];
-                    var fileRejections = [];
-                    files.forEach(function(file) {
-                        var _fileAccepted = fileAccepted(file, accept),
-                            _fileAccepted2 = _slicedToArray$8(_fileAccepted, 2),
-                            accepted = _fileAccepted2[0],
-                            acceptError = _fileAccepted2[1];
-                        var _fileMatchSize = fileMatchSize(file, minSize, maxSize),
-                            _fileMatchSize2 = _slicedToArray$8(_fileMatchSize, 2),
-                            sizeMatch = _fileMatchSize2[0],
-                            sizeError = _fileMatchSize2[1];
-                        if (accepted && sizeMatch) {
-                            acceptedFiles.push(file);
-                        } else {
-                            var errors = [acceptError, sizeError].filter(function(e3) {
-                                return e3;
-                            });
-                            fileRejections.push({
-                                file,
-                                errors
-                            });
-                        }
-                    });
-                    if (!multiple && acceptedFiles.length > 1) {
-                        acceptedFiles.forEach(function(file) {
-                            fileRejections.push({
-                                file,
-                                errors: [TOO_MANY_FILES_REJECTION]
-                            });
-                        });
-                        acceptedFiles.splice(0);
-                    }
-                    dispatch2({
-                        acceptedFiles,
-                        fileRejections,
-                        type: "setFiles"
-                    });
-                    if (onDrop) {
-                        onDrop(acceptedFiles, fileRejections, event2);
-                    }
-                    if (fileRejections.length > 0 && onDropRejected) {
-                        onDropRejected(fileRejections, event2);
-                    }
-                    if (acceptedFiles.length > 0 && onDropAccepted) {
-                        onDropAccepted(acceptedFiles, event2);
-                    }
-                });
-            }
-            dispatch2({
-                type: "reset"
-            });
-        }, [multiple, accept, minSize, maxSize, getFilesFromEvent, onDrop, onDropAccepted, onDropRejected, noDragEventsBubbling]);
-        var composeHandler = function composeHandler2(fn2) {
-            return disabled2 ? null : fn2;
-        };
-        var composeKeyboardHandler = function composeKeyboardHandler2(fn2) {
-            return noKeyboard ? null : composeHandler(fn2);
-        };
-        var composeDragHandler = function composeDragHandler2(fn2) {
-            return noDrag ? null : composeHandler(fn2);
-        };
-        var stopPropagation = function stopPropagation2(event2) {
-            if (noDragEventsBubbling) {
-                event2.stopPropagation();
-            }
-        };
-        var getRootProps = React.useMemo(function() {
-            return function() {
-                var _ref3 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
-                    _ref3$refKey = _ref3.refKey,
-                    refKey = _ref3$refKey === void 0 ? "ref" : _ref3$refKey,
-                    onKeyDown = _ref3.onKeyDown,
-                    onFocus = _ref3.onFocus,
-                    onBlur = _ref3.onBlur,
-                    onClick = _ref3.onClick,
-                    onDragEnter2 = _ref3.onDragEnter,
-                    onDragOver2 = _ref3.onDragOver,
-                    onDragLeave2 = _ref3.onDragLeave,
-                    onDrop2 = _ref3.onDrop,
-                    rest = _objectWithoutProperties$1(_ref3, ["refKey", "onKeyDown", "onFocus", "onBlur", "onClick", "onDragEnter", "onDragOver", "onDragLeave", "onDrop"]);
-                return _objectSpread$5(_defineProperty$n({
-                    onKeyDown: composeKeyboardHandler(composeEventHandlers(onKeyDown, onKeyDownCb)),
-                    onFocus: composeKeyboardHandler(composeEventHandlers(onFocus, onFocusCb)),
-                    onBlur: composeKeyboardHandler(composeEventHandlers(onBlur, onBlurCb)),
-                    onClick: composeHandler(composeEventHandlers(onClick, onClickCb)),
-                    onDragEnter: composeDragHandler(composeEventHandlers(onDragEnter2, onDragEnterCb)),
-                    onDragOver: composeDragHandler(composeEventHandlers(onDragOver2, onDragOverCb)),
-                    onDragLeave: composeDragHandler(composeEventHandlers(onDragLeave2, onDragLeaveCb)),
-                    onDrop: composeDragHandler(composeEventHandlers(onDrop2, onDropCb))
-                }, refKey, rootRef), !disabled2 && !noKeyboard ? {
-                    tabIndex: 0
-                } : {}, {}, rest);
-            };
-        }, [rootRef, onKeyDownCb, onFocusCb, onBlurCb, onClickCb, onDragEnterCb, onDragOverCb, onDragLeaveCb, onDropCb, noKeyboard, noDrag, disabled2]);
-        var onInputElementClick = React.useCallback(function(event2) {
-            event2.stopPropagation();
-        }, []);
-        var getInputProps = React.useMemo(function() {
-            return function() {
-                var _ref4 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
-                    _ref4$refKey = _ref4.refKey,
-                    refKey = _ref4$refKey === void 0 ? "ref" : _ref4$refKey,
-                    onChange2 = _ref4.onChange,
-                    onClick = _ref4.onClick,
-                    rest = _objectWithoutProperties$1(_ref4, ["refKey", "onChange", "onClick"]);
-                var inputProps = _defineProperty$n({
-                    accept,
-                    multiple,
-                    type: "file",
-                    style: {
-                        display: "none"
-                    },
-                    onChange: composeHandler(composeEventHandlers(onChange2, onDropCb)),
-                    onClick: composeHandler(composeEventHandlers(onClick, onInputElementClick)),
-                    autoComplete: "off",
-                    tabIndex: -1
-                }, refKey, inputRef);
-                return _objectSpread$5({}, inputProps, {}, rest);
-            };
-        }, [inputRef, accept, multiple, onDropCb, disabled2]);
-        var fileCount = draggedFiles.length;
-        var isDragAccept = fileCount > 0 && allFilesAccepted({
-            files: draggedFiles,
-            accept,
-            minSize,
-            maxSize,
-            multiple
-        });
-        var isDragReject = fileCount > 0 && !isDragAccept;
-        return _objectSpread$5({}, state, {
-            isDragAccept,
-            isDragReject,
-            isFocused: isFocused && !disabled2,
-            getRootProps,
-            getInputProps,
-            rootRef,
-            inputRef,
-            open: composeHandler(openFileDialog)
-        });
-    }
-
-    function reducer(state, action) {
-        switch (action.type) {
-            case "focus":
-                return _objectSpread$5({}, state, {
-                    isFocused: true
-                });
-            case "blur":
-                return _objectSpread$5({}, state, {
-                    isFocused: false
-                });
-            case "openDialog":
-                return _objectSpread$5({}, state, {
-                    isFileDialogActive: true
-                });
-            case "closeDialog":
-                return _objectSpread$5({}, state, {
-                    isFileDialogActive: false
-                });
-            case "setDraggedFiles":
-                var isDragActive = action.isDragActive,
-                    draggedFiles = action.draggedFiles;
-                return _objectSpread$5({}, state, {
-                    draggedFiles,
-                    isDragActive
-                });
-            case "setFiles":
-                return _objectSpread$5({}, state, {
-                    acceptedFiles: action.acceptedFiles,
-                    fileRejections: action.fileRejections
-                });
-            case "reset":
-                return _objectSpread$5({}, state, {
-                    isFileDialogActive: false,
-                    isDragActive: false,
-                    draggedFiles: [],
-                    acceptedFiles: [],
-                    fileRejections: []
-                });
-            default:
-                return state;
-        }
-    }
-    const DROPZONE_ALLOWED_MIME_TYPES = ".csv, text/csv, application/vnd.openxmlformats-officedocument.spreadsheetml.sheet, application/vnd.ms-excel, application/csv, text/x-csv, application/x-csv, text/comma-separated-values, text/x-comma-separated-values";
-    const Dropzone = styled__default.default.div`
-    display: flex;
-    flex: 1 1 auto;
-    align-items: center;
-    justify-content: center;
-
-    margin-top: 20px;
-
-    color: ${(props) => props.theme.colors.text};
-
-    border: 1px dashed ${(props) => props.isDragActive ? props.theme.colors.primary : props.theme.colors.grey3};
-    border-radius: 0.25rem;
-
-    :hover {
-        background-color: ${(props) => props.theme.colors.grey1};
-    }
-
-    :active,
-    :focus {
-        background-color: ${(props) => props.theme.colors.grey2};
-    }
-`;
-    const DropzoneMessage = styled__default.default.span`
-    max-width: 400px;
-    padding: 1.5rem;
-
-    font-family: Manrope, sans-serif;
-    font-weight: 300;
-    text-align: center;
-`;
-
-    function UploadDropzone$1(props) {
-        var _a3;
-        React.useEffect(() => {
-            if (!props.enablePaste) {
-                return;
-            }
-            const handlePaste = (ev) => {
-                const blob = new Blob([ev.clipboardData.getData("Text")], {
-                    type: "text/plain"
-                });
-                const file = new File([blob], "pasted_data", {
-                    type: "text/plain"
-                });
-                props.onDrop([file]);
-            };
-            document.addEventListener("paste", handlePaste);
-            return () => document.removeEventListener("paste", handlePaste);
-        }, [props]);
-        const {
-            getRootProps,
-            getInputProps,
-            isDragActive
-        } = useDropzone({
-            accept: (_a3 = props.accept) !== null && _a3 !== void 0 ? _a3 : DROPZONE_ALLOWED_MIME_TYPES,
-            multiple: false,
-            onDrop: props.onDrop
-        });
-        return jsxRuntime.exports.jsxs(Dropzone, Object.assign({}, getRootProps(), {
-            className: props.className,
-            isDragActive,
-            style: props.style,
-            children: [jsxRuntime.exports.jsx("input", Object.assign({}, getInputProps())), jsxRuntime.exports.jsxs(DropzoneMessage, {
-                children: ["Drop your file, ", jsxRuntime.exports.jsx("br", {}), "paste it ", jsxRuntime.exports.jsx("br", {}), "or click here to upload"]
-            })]
-        }));
-    }
-    styled__default.default.div`
-    display: flex;
-    flex-direction: column;
-
-    width: 100%;
-    padding: 1rem;
-
-    color: ${(props) => props.theme.colors.error};
-
-    background-color: ${(props) => props.theme.colors.background};
-`;
-    styled__default.default.div`
-    overflow: scroll;
-    display: flex;
-    flex-direction: column;
-
-    width: 100%;
-    max-height: 125px;
-    margin: 2rem 0;
-    padding: 0.5rem;
-
-    color: ${(props) => props.theme.colors.background};
-
-    background-color: ${(props) => props.theme.colors.errorHover};
-`;
-    styled__default.default.p`
-    color: ${(props) => props.theme.colors.error};
-`;
-    const NodeContent = styled__default.default.li`
-    margin-left: 0.35rem;
-    border-left: thin solid ${(props) => props.theme.colors.grey6};
-
-    &::before {
-        content: '';
-
-        display: inline-block;
-
-        width: 0.9rem;
-        height: 0.8rem;
-        margin-right: 0.1rem;
-
-        vertical-align: top;
-
-        border-bottom: thin solid ${(props) => props.theme.colors.grey6};
-    }
-
-    &:last-child {
-        border-left: none;
-
-        &::before {
-            border-left: thin solid ${(props) => props.theme.colors.grey6};
-        }
-    }
-`;
-    const Cell$1 = styled__default.default.span`
-    cursor: ${(props) => props.selectionAllowed ? "pointer" : "normal"};
-    font-weight: ${(props) => props.isLeaf ? 300 : 400};
-    color: ${(props) => {
-    if (props.selected) {
-      return props.theme.colors.primary;
-    }
-    return props.isLeaf ? props.theme.colors.grey6 : props.theme.colors.grey5;
-  }};
-`;
-    const CircleIcon = styled__default.default(Circle$1)`
-    width: 0.5rem;
-    height: 0.5rem;
-    margin-right: 0.4rem;
-
-    color: ${(props) => props.selected ? props.theme.colors.primary : props.theme.colors.grey6};
-    vertical-align: middle;
-`;
-    const grow = styled.keyframes`
-    0% {
-        transform: scaleY(0);
-        opacity: 0;
-    }
-    100% {
-        transform: scaleY(1);
-        opacity: 1;
-    }
-`;
-    const contract = styled.keyframes`
-    100% {
-        transform: scaleY(1);
-        opacity: 1;
-    }
-    0% {
-        transform: scaleY(0);
-        opacity: 0;
-    }
-`;
-    const NodeWrapper = styled__default.default.ul`
-    transform-origin: top center;
-
-    display: ${(props) => props.open ? "block" : "none"};
-
-    margin: 0;
-    margin-left: 1rem;
-    padding: 0;
-    padding-bottom: 1rem;
-
-    list-style: none;
-
-    animation: ${(props) => props.open ? grow : contract} 300ms
-        ${(props) => props.open ? "ease-out forwards" : "ease-in forwards"};
-`;
-
-    function Branch(props) {
-        const theme2 = useClTheme();
-        const [open, setOpen] = React.useState(props.open || false);
-        const toggle = () => {
-            if (props.content) {
-                setOpen(!open);
-            }
-        };
-        const select = () => {
-            props.selectNode(props.content.id);
-        };
-        const selectionAllowed = props.allowSelectCategory && props.content.children && props.content.children.length > 0 || props.allowSelectLeaf && (!props.content.children || props.content.children.length === 0);
-        return jsxRuntime.exports.jsxs(NodeContent, {
-            className: props.className,
-            style: props.style,
-            children: [jsxRuntime.exports.jsx(CircleIcon, {
-                selected: props.content.id === props.selectedNodeId
-            }), jsxRuntime.exports.jsx(Cell$1, {
-                isLeaf: !props.content.children || props.content.children.length === 0,
-                onClick: selectionAllowed ? select : toggle,
-                selected: props.content.id === props.selectedNodeId,
-                selectionAllowed,
-                children: props.content.label
-            }), props.content.children && props.content.children.length > 0 && jsxRuntime.exports.jsx(Chevron$2, {
-                isOpen: open,
-                onClick: toggle,
-                style: {
-                    color: theme2.colors.grey5,
-                    cursor: "pointer",
-                    height: "0.8rem",
-                    marginLeft: "0.5rem",
-                    verticalAlign: "middle",
-                    width: "0.8rem"
-                }
-            }), jsxRuntime.exports.jsx(NodeWrapper, {
-                open,
-                children: props.content.children && props.content.children.length > 0 && props.content.children.map((nodeObj) => jsxRuntime.exports.jsx(Branch, {
-                    allowSelectCategory: props.allowSelectCategory,
-                    allowSelectLeaf: props.allowSelectLeaf,
-                    content: nodeObj,
-                    selectCategory: props.selectCategory,
-                    selectNode: props.selectNode,
-                    selectedNodeId: props.selectedNodeId
-                }, nodeObj.id))
-            })]
-        });
-    }
-    const Wrapper$8 = styled__default.default.div`
-    overflow: scroll;
-`;
-    const Root = styled__default.default.div`
-    cursor: pointer;
-    margin-left: 1rem;
-`;
-
-    function HierarchySelector$1(props) {
-        const theme2 = useClTheme();
-        const [rootOpen, setRootOpen] = React.useState(props.rootOpen || false);
-        const [selectedNodeId, setSelectedNodeId] = React.useState(props.selected);
-        React.useEffect(() => {
-            if (props.selected) {
-                setSelectedNodeId(props.selected);
-            }
-        }, [props.selected]);
-        const toggle = () => {
-            setRootOpen(!rootOpen);
-        };
-        const selectNode = (nodeId) => {
-            var _a3;
-            setSelectedNodeId(nodeId);
-            (_a3 = props.onSelect) === null || _a3 === void 0 ? void 0 : _a3.call(props, nodeId);
-        };
-        const {
-            label,
-            id: id2,
-            children: children2
-        } = props.rootNode;
-        return jsxRuntime.exports.jsxs(Wrapper$8, {
-            className: props.className,
-            style: props.style,
-            children: [jsxRuntime.exports.jsxs(Root, {
-                children: [jsxRuntime.exports.jsx(CircleIcon, {
-                    selected: id2 === selectedNodeId
-                }), jsxRuntime.exports.jsx(Cell$1, {
-                    onClick: props.allowSelectCategory || children2.length === 0 ? () => selectNode(id2) : toggle,
-                    selected: id2 === selectedNodeId,
-                    children: label
-                }), children2.length > 0 && jsxRuntime.exports.jsx(Chevron$2, {
-                    isOpen: rootOpen,
-                    onClick: toggle,
-                    style: {
-                        color: theme2.colors.grey5,
-                        cursor: "pointer",
-                        height: "0.8rem",
-                        marginLeft: "0.5rem",
-                        verticalAlign: "middle",
-                        width: "0.8rem"
-                    }
-                })]
-            }), jsxRuntime.exports.jsx(NodeWrapper, {
-                open: rootOpen,
-                children: children2 && children2.map((nodeObj) => jsxRuntime.exports.jsx(Branch, {
-                    allowSelectCategory: props.allowSelectCategory,
-                    allowSelectLeaf: props.allowSelectLeaf,
-                    content: nodeObj,
-                    open: rootOpen,
-                    selectNode,
-                    selectedNodeId
-                }, nodeObj.id))
-            })]
-        });
-    }
-    const Background$1 = styled__default.default.div`
-    position: fixed;
-    z-index: 2000;
-    top: 0;
-    left: 0;
-
-    display: flex;
-    align-items: center;
-    justify-content: center;
-
-    width: 100%;
-    height: 100%;
-
-    opacity: ${(props) => props.render ? 1 : 0};
-    background-color: ${(props) => props.theme.colors.modalBg};
-
-    transition: opacity ease-in 0.1s;
-`;
-    const ModalWrapper = styled__default.default.div`
-    overflow: hidden;
-    display: inline-flex;
-    flex-direction: column;
-
-    min-width: 20rem;
-    max-width: 80vw;
-    min-height: 10rem;
-    max-height: 80vh;
-    margin-top: ${(props) => props.render ? 0 : "-50px"};
-    padding: 1.75rem;
-
-    font-size: ${(props) => props.theme.font.size};
-
-    background-color: ${(props) => props.theme.colors.grey1};
-    border-radius: 0.25rem;
-    box-shadow: ${(props) => props.theme.shadow.medium};
-
-    transition: margin-top ease-in 0.1s;
-`;
-    styled__default.default.div`
-    display: flex;
-    flex: 0 0 auto;
-    justify-content: space-between;
-    margin-top: 1rem;
-`;
-    styled__default.default.div`
-    display: flex;
-    flex: 0 0 auto;
-    flex-direction: ${(props) => props.flexDirection || "column"};
-    justify-content: space-between;
-
-    margin-bottom: 1rem;
-`;
-
-    function Modal$1(props) {
-        var _a3;
-        const [mounted, setMounted] = React.useState(false);
-        const [renderModal, setRenderModal] = React.useState(false);
-        React.useEffect(() => {
-            setRenderModal(props.render);
-        }, [props.render]);
-        React.useEffect(() => {
-            if (renderModal) {
-                const keyHandler = (e3) => {
-                    if (e3.key === Key.ESCAPE && props.onAttemptClose) {
-                        props.onAttemptClose();
-                    }
-                };
-                document.addEventListener("keydown", keyHandler);
-                return () => {
-                    document.removeEventListener("keydown", keyHandler);
-                };
-            }
-        }, [renderModal, props.onAttemptClose]);
-        if (!props.render && !mounted) {
-            return null;
-        }
-        const onTransitionEnd = () => {
-            setMounted(props.render);
-            if (!props.render && props.onClosed) {
-                props.onClosed();
-            }
-        };
-        const stopPropagation = (e3) => {
-            e3.stopPropagation();
-        };
-        return ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(Background$1, {
-            id: props.id,
-            onClick: props.onAttemptClose,
-            onTransitionEnd,
-            render: renderModal,
-            children: jsxRuntime.exports.jsx(ModalWrapper, {
-                className: `cl-modal-content ${(_a3 = props.className) !== null && _a3 !== void 0 ? _a3 : ""}`,
-                onClick: stopPropagation,
-                render: renderModal,
-                style: props.style,
-                children: props.children
-            })
-        }), document.body);
-    }
-
-    function getNodeName(node2) {
-        if (isNode(node2)) {
-            return (node2.nodeName || "").toLowerCase();
-        }
-        return "#document";
-    }
-
-    function getWindow(node2) {
-        var _node$ownerDocument;
-        return (node2 == null || (_node$ownerDocument = node2.ownerDocument) == null ? void 0 : _node$ownerDocument.defaultView) || window;
-    }
-
-    function getDocumentElement(node2) {
-        var _ref2;
-        return (_ref2 = (isNode(node2) ? node2.ownerDocument : node2.document) || window.document) == null ? void 0 : _ref2.documentElement;
-    }
-
-    function isNode(value) {
-        return value instanceof Node || value instanceof getWindow(value).Node;
-    }
-
-    function isElement$1(value) {
-        return value instanceof Element || value instanceof getWindow(value).Element;
-    }
-
-    function isHTMLElement(value) {
-        return value instanceof HTMLElement || value instanceof getWindow(value).HTMLElement;
-    }
-
-    function isShadowRoot(value) {
-        if (typeof ShadowRoot === "undefined") {
-            return false;
-        }
-        return value instanceof ShadowRoot || value instanceof getWindow(value).ShadowRoot;
-    }
-
-    function isOverflowElement(element2) {
-        const {
-            overflow,
-            overflowX,
-            overflowY,
-            display
-        } = getComputedStyle$1(element2);
-        return /auto|scroll|overlay|hidden|clip/.test(overflow + overflowY + overflowX) && !["inline", "contents"].includes(display);
-    }
-
-    function isTableElement(element2) {
-        return ["table", "td", "th"].includes(getNodeName(element2));
-    }
-
-    function isContainingBlock(element2) {
-        const webkit2 = isWebKit();
-        const css2 = getComputedStyle$1(element2);
-        return css2.transform !== "none" || css2.perspective !== "none" || (css2.containerType ? css2.containerType !== "normal" : false) || !webkit2 && (css2.backdropFilter ? css2.backdropFilter !== "none" : false) || !webkit2 && (css2.filter ? css2.filter !== "none" : false) || ["transform", "perspective", "filter"].some((value) => (css2.willChange || "").includes(value)) || ["paint", "layout", "strict", "content"].some((value) => (css2.contain || "").includes(value));
-    }
-
-    function getContainingBlock(element2) {
-        let currentNode = getParentNode(element2);
-        while (isHTMLElement(currentNode) && !isLastTraversableNode(currentNode)) {
-            if (isContainingBlock(currentNode)) {
-                return currentNode;
-            } else {
-                currentNode = getParentNode(currentNode);
-            }
-        }
-        return null;
-    }
-
-    function isWebKit() {
-        if (typeof CSS === "undefined" || !CSS.supports)
-            return false;
-        return CSS.supports("-webkit-backdrop-filter", "none");
-    }
-
-    function isLastTraversableNode(node2) {
-        return ["html", "body", "#document"].includes(getNodeName(node2));
-    }
-
-    function getComputedStyle$1(element2) {
-        return getWindow(element2).getComputedStyle(element2);
-    }
-
-    function getNodeScroll(element2) {
-        if (isElement$1(element2)) {
-            return {
-                scrollLeft: element2.scrollLeft,
-                scrollTop: element2.scrollTop
-            };
-        }
-        return {
-            scrollLeft: element2.pageXOffset,
-            scrollTop: element2.pageYOffset
-        };
-    }
-
-    function getParentNode(node2) {
-        if (getNodeName(node2) === "html") {
-            return node2;
-        }
-        const result = node2.assignedSlot || node2.parentNode || isShadowRoot(node2) && node2.host || getDocumentElement(node2);
-        return isShadowRoot(result) ? result.host : result;
-    }
-
-    function getNearestOverflowAncestor(node2) {
-        const parentNode = getParentNode(node2);
-        if (isLastTraversableNode(parentNode)) {
-            return node2.ownerDocument ? node2.ownerDocument.body : node2.body;
-        }
-        if (isHTMLElement(parentNode) && isOverflowElement(parentNode)) {
-            return parentNode;
-        }
-        return getNearestOverflowAncestor(parentNode);
-    }
-
-    function getOverflowAncestors(node2, list2, traverseIframes) {
-        var _node$ownerDocument2;
-        if (list2 === void 0) {
-            list2 = [];
-        }
-        if (traverseIframes === void 0) {
-            traverseIframes = true;
-        }
-        const scrollableAncestor = getNearestOverflowAncestor(node2);
-        const isBody = scrollableAncestor === ((_node$ownerDocument2 = node2.ownerDocument) == null ? void 0 : _node$ownerDocument2.body);
-        const win = getWindow(scrollableAncestor);
-        if (isBody) {
-            return list2.concat(win, win.visualViewport || [], isOverflowElement(scrollableAncestor) ? scrollableAncestor : [], win.frameElement && traverseIframes ? getOverflowAncestors(win.frameElement) : []);
-        }
-        return list2.concat(scrollableAncestor, getOverflowAncestors(scrollableAncestor, [], traverseIframes));
-    }
-    const sides = ["top", "right", "bottom", "left"];
-    const alignments = ["start", "end"];
-    const placements = /* @__PURE__ */ sides.reduce((acc, side) => acc.concat(side, side + "-" + alignments[0], side + "-" + alignments[1]), []);
-    const min$1 = Math.min;
-    const max$2 = Math.max;
-    const round$2 = Math.round;
-    const floor = Math.floor;
-    const createCoords = (v3) => ({
-        x: v3,
-        y: v3
-    });
-    const oppositeSideMap = {
-        left: "right",
-        right: "left",
-        bottom: "top",
-        top: "bottom"
-    };
-    const oppositeAlignmentMap = {
-        start: "end",
-        end: "start"
-    };
-
-    function clamp$1(start2, value, end2) {
-        return max$2(start2, min$1(value, end2));
-    }
-
-    function evaluate(value, param) {
-        return typeof value === "function" ? value(param) : value;
-    }
-
-    function getSide(placement) {
-        return placement.split("-")[0];
-    }
-
-    function getAlignment(placement) {
-        return placement.split("-")[1];
-    }
-
-    function getOppositeAxis(axis) {
-        return axis === "x" ? "y" : "x";
-    }
-
-    function getAxisLength(axis) {
-        return axis === "y" ? "height" : "width";
-    }
-
-    function getSideAxis(placement) {
-        return ["top", "bottom"].includes(getSide(placement)) ? "y" : "x";
-    }
-
-    function getAlignmentAxis(placement) {
-        return getOppositeAxis(getSideAxis(placement));
-    }
-
-    function getAlignmentSides(placement, rects, rtl) {
-        if (rtl === void 0) {
-            rtl = false;
-        }
-        const alignment = getAlignment(placement);
-        const alignmentAxis = getAlignmentAxis(placement);
-        const length = getAxisLength(alignmentAxis);
-        let mainAlignmentSide = alignmentAxis === "x" ? alignment === (rtl ? "end" : "start") ? "right" : "left" : alignment === "start" ? "bottom" : "top";
-        if (rects.reference[length] > rects.floating[length]) {
-            mainAlignmentSide = getOppositePlacement(mainAlignmentSide);
-        }
-        return [mainAlignmentSide, getOppositePlacement(mainAlignmentSide)];
-    }
-
-    function getExpandedPlacements(placement) {
-        const oppositePlacement = getOppositePlacement(placement);
-        return [getOppositeAlignmentPlacement(placement), oppositePlacement, getOppositeAlignmentPlacement(oppositePlacement)];
-    }
-
-    function getOppositeAlignmentPlacement(placement) {
-        return placement.replace(/start|end/g, (alignment) => oppositeAlignmentMap[alignment]);
-    }
-
-    function getSideList(side, isStart, rtl) {
-        const lr2 = ["left", "right"];
-        const rl = ["right", "left"];
-        const tb = ["top", "bottom"];
-        const bt2 = ["bottom", "top"];
-        switch (side) {
-            case "top":
-            case "bottom":
-                if (rtl)
-                    return isStart ? rl : lr2;
-                return isStart ? lr2 : rl;
-            case "left":
-            case "right":
-                return isStart ? tb : bt2;
-            default:
-                return [];
-        }
-    }
-
-    function getOppositeAxisPlacements(placement, flipAlignment, direction, rtl) {
-        const alignment = getAlignment(placement);
-        let list2 = getSideList(getSide(placement), direction === "start", rtl);
-        if (alignment) {
-            list2 = list2.map((side) => side + "-" + alignment);
-            if (flipAlignment) {
-                list2 = list2.concat(list2.map(getOppositeAlignmentPlacement));
-            }
-        }
-        return list2;
-    }
-
-    function getOppositePlacement(placement) {
-        return placement.replace(/left|right|bottom|top/g, (side) => oppositeSideMap[side]);
-    }
-
-    function expandPaddingObject(padding) {
-        return {
-            top: 0,
-            right: 0,
-            bottom: 0,
-            left: 0,
-            ...padding
-        };
-    }
-
-    function getPaddingObject(padding) {
-        return typeof padding !== "number" ? expandPaddingObject(padding) : {
-            top: padding,
-            right: padding,
-            bottom: padding,
-            left: padding
-        };
-    }
-
-    function rectToClientRect(rect) {
-        return {
-            ...rect,
-            top: rect.y,
-            left: rect.x,
-            right: rect.x + rect.width,
-            bottom: rect.y + rect.height
-        };
-    }
-
-    function computeCoordsFromPlacement(_ref2, placement, rtl) {
-        let {
-            reference: reference2,
-            floating
-        } = _ref2;
-        const sideAxis = getSideAxis(placement);
-        const alignmentAxis = getAlignmentAxis(placement);
-        const alignLength = getAxisLength(alignmentAxis);
-        const side = getSide(placement);
-        const isVertical = sideAxis === "y";
-        const commonX = reference2.x + reference2.width / 2 - floating.width / 2;
-        const commonY = reference2.y + reference2.height / 2 - floating.height / 2;
-        const commonAlign = reference2[alignLength] / 2 - floating[alignLength] / 2;
-        let coords;
-        switch (side) {
-            case "top":
-                coords = {
-                    x: commonX,
-                    y: reference2.y - floating.height
-                };
-                break;
-            case "bottom":
-                coords = {
-                    x: commonX,
-                    y: reference2.y + reference2.height
-                };
-                break;
-            case "right":
-                coords = {
-                    x: reference2.x + reference2.width,
-                    y: commonY
-                };
-                break;
-            case "left":
-                coords = {
-                    x: reference2.x - floating.width,
-                    y: commonY
-                };
-                break;
-            default:
-                coords = {
-                    x: reference2.x,
-                    y: reference2.y
-                };
-        }
-        switch (getAlignment(placement)) {
-            case "start":
-                coords[alignmentAxis] -= commonAlign * (rtl && isVertical ? -1 : 1);
-                break;
-            case "end":
-                coords[alignmentAxis] += commonAlign * (rtl && isVertical ? -1 : 1);
-                break;
-        }
-        return coords;
-    }
-    const computePosition$1 = async (reference2, floating, config2) => {
-        const {
-            placement = "bottom",
-                strategy = "absolute",
-                middleware = [],
-                platform: platform2
-        } = config2;
-        const validMiddleware = middleware.filter(Boolean);
-        const rtl = await (platform2.isRTL == null ? void 0 : platform2.isRTL(floating));
-        let rects = await platform2.getElementRects({
-            reference: reference2,
-            floating,
-            strategy
-        });
-        let {
-            x: x2,
-            y: y2
-        } = computeCoordsFromPlacement(rects, placement, rtl);
-        let statefulPlacement = placement;
-        let middlewareData = {};
-        let resetCount = 0;
-        for (let i2 = 0; i2 < validMiddleware.length; i2++) {
-            const {
-                name: name2,
-                fn: fn2
-            } = validMiddleware[i2];
-            const {
-                x: nextX,
-                y: nextY,
-                data: data2,
-                reset: reset2
-            } = await fn2({
-                x: x2,
-                y: y2,
-                initialPlacement: placement,
-                placement: statefulPlacement,
-                strategy,
-                middlewareData,
-                rects,
-                platform: platform2,
-                elements: {
-                    reference: reference2,
-                    floating
-                }
-            });
-            x2 = nextX != null ? nextX : x2;
-            y2 = nextY != null ? nextY : y2;
-            middlewareData = {
-                ...middlewareData,
-                [name2]: {
-                    ...middlewareData[name2],
-                    ...data2
-                }
-            };
-            if (reset2 && resetCount <= 50) {
-                resetCount++;
-                if (typeof reset2 === "object") {
-                    if (reset2.placement) {
-                        statefulPlacement = reset2.placement;
-                    }
-                    if (reset2.rects) {
-                        rects = reset2.rects === true ? await platform2.getElementRects({
-                            reference: reference2,
-                            floating,
-                            strategy
-                        }) : reset2.rects;
-                    }
-                    ({
-                        x: x2,
-                        y: y2
-                    } = computeCoordsFromPlacement(rects, statefulPlacement, rtl));
-                }
-                i2 = -1;
-            }
-        }
-        return {
-            x: x2,
-            y: y2,
-            placement: statefulPlacement,
-            strategy,
-            middlewareData
-        };
-    };
-    async function detectOverflow(state, options) {
-        var _await$platform$isEle;
-        if (options === void 0) {
-            options = {};
-        }
-        const {
-            x: x2,
-            y: y2,
-            platform: platform2,
-            rects,
-            elements,
-            strategy
-        } = state;
-        const {
-            boundary = "clippingAncestors",
-                rootBoundary = "viewport",
-                elementContext = "floating",
-                altBoundary = false,
-                padding = 0
-        } = evaluate(options, state);
-        const paddingObject = getPaddingObject(padding);
-        const altContext = elementContext === "floating" ? "reference" : "floating";
-        const element2 = elements[altBoundary ? altContext : elementContext];
-        const clippingClientRect = rectToClientRect(await platform2.getClippingRect({
-            element: ((_await$platform$isEle = await (platform2.isElement == null ? void 0 : platform2.isElement(element2))) != null ? _await$platform$isEle : true) ? element2 : element2.contextElement || await (platform2.getDocumentElement == null ? void 0 : platform2.getDocumentElement(elements.floating)),
-            boundary,
-            rootBoundary,
-            strategy
-        }));
-        const rect = elementContext === "floating" ? {
-            ...rects.floating,
-            x: x2,
-            y: y2
-        } : rects.reference;
-        const offsetParent = await (platform2.getOffsetParent == null ? void 0 : platform2.getOffsetParent(elements.floating));
-        const offsetScale = await (platform2.isElement == null ? void 0 : platform2.isElement(offsetParent)) ? await (platform2.getScale == null ? void 0 : platform2.getScale(offsetParent)) || {
-            x: 1,
-            y: 1
-        } : {
-            x: 1,
-            y: 1
-        };
-        const elementClientRect = rectToClientRect(platform2.convertOffsetParentRelativeRectToViewportRelativeRect ? await platform2.convertOffsetParentRelativeRectToViewportRelativeRect({
-            elements,
-            rect,
-            offsetParent,
-            strategy
-        }) : rect);
-        return {
-            top: (clippingClientRect.top - elementClientRect.top + paddingObject.top) / offsetScale.y,
-            bottom: (elementClientRect.bottom - clippingClientRect.bottom + paddingObject.bottom) / offsetScale.y,
-            left: (clippingClientRect.left - elementClientRect.left + paddingObject.left) / offsetScale.x,
-            right: (elementClientRect.right - clippingClientRect.right + paddingObject.right) / offsetScale.x
-        };
-    }
-    const arrow = (options) => ({
-        name: "arrow",
-        options,
-        async fn(state) {
-            const {
-                x: x2,
-                y: y2,
-                placement,
-                rects,
-                platform: platform2,
-                elements,
-                middlewareData
-            } = state;
-            const {
-                element: element2,
-                padding = 0
-            } = evaluate(options, state) || {};
-            if (element2 == null) {
-                return {};
-            }
-            const paddingObject = getPaddingObject(padding);
-            const coords = {
-                x: x2,
-                y: y2
-            };
-            const axis = getAlignmentAxis(placement);
-            const length = getAxisLength(axis);
-            const arrowDimensions = await platform2.getDimensions(element2);
-            const isYAxis = axis === "y";
-            const minProp = isYAxis ? "top" : "left";
-            const maxProp = isYAxis ? "bottom" : "right";
-            const clientProp = isYAxis ? "clientHeight" : "clientWidth";
-            const endDiff = rects.reference[length] + rects.reference[axis] - coords[axis] - rects.floating[length];
-            const startDiff = coords[axis] - rects.reference[axis];
-            const arrowOffsetParent = await (platform2.getOffsetParent == null ? void 0 : platform2.getOffsetParent(element2));
-            let clientSize = arrowOffsetParent ? arrowOffsetParent[clientProp] : 0;
-            if (!clientSize || !await (platform2.isElement == null ? void 0 : platform2.isElement(arrowOffsetParent))) {
-                clientSize = elements.floating[clientProp] || rects.floating[length];
-            }
-            const centerToReference = endDiff / 2 - startDiff / 2;
-            const largestPossiblePadding = clientSize / 2 - arrowDimensions[length] / 2 - 1;
-            const minPadding = min$1(paddingObject[minProp], largestPossiblePadding);
-            const maxPadding = min$1(paddingObject[maxProp], largestPossiblePadding);
-            const min$1$1 = minPadding;
-            const max2 = clientSize - arrowDimensions[length] - maxPadding;
-            const center2 = clientSize / 2 - arrowDimensions[length] / 2 + centerToReference;
-            const offset2 = clamp$1(min$1$1, center2, max2);
-            const shouldAddOffset = !middlewareData.arrow && getAlignment(placement) != null && center2 !== offset2 && rects.reference[length] / 2 - (center2 < min$1$1 ? minPadding : maxPadding) - arrowDimensions[length] / 2 < 0;
-            const alignmentOffset = shouldAddOffset ? center2 < min$1$1 ? center2 - min$1$1 : center2 - max2 : 0;
-            return {
-                [axis]: coords[axis] + alignmentOffset,
-                data: {
-                    [axis]: offset2,
-                    centerOffset: center2 - offset2 - alignmentOffset,
-                    ...shouldAddOffset && {
-                        alignmentOffset
-                    }
-                },
-                reset: shouldAddOffset
-            };
-        }
-    });
-
-    function getPlacementList(alignment, autoAlignment, allowedPlacements) {
-        const allowedPlacementsSortedByAlignment = alignment ? [...allowedPlacements.filter((placement) => getAlignment(placement) === alignment), ...allowedPlacements.filter((placement) => getAlignment(placement) !== alignment)] : allowedPlacements.filter((placement) => getSide(placement) === placement);
-        return allowedPlacementsSortedByAlignment.filter((placement) => {
-            if (alignment) {
-                return getAlignment(placement) === alignment || (autoAlignment ? getOppositeAlignmentPlacement(placement) !== placement : false);
-            }
-            return true;
-        });
-    }
-    const autoPlacement = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            name: "autoPlacement",
-            options,
-            async fn(state) {
-                var _middlewareData$autoP, _middlewareData$autoP2, _placementsThatFitOnE;
-                const {
-                    rects,
-                    middlewareData,
-                    placement,
-                    platform: platform2,
-                    elements
-                } = state;
-                const {
-                    crossAxis = false,
-                        alignment,
-                        allowedPlacements = placements,
-                        autoAlignment = true,
-                        ...detectOverflowOptions
-                } = evaluate(options, state);
-                const placements$12 = alignment !== void 0 || allowedPlacements === placements ? getPlacementList(alignment || null, autoAlignment, allowedPlacements) : allowedPlacements;
-                const overflow = await detectOverflow(state, detectOverflowOptions);
-                const currentIndex = ((_middlewareData$autoP = middlewareData.autoPlacement) == null ? void 0 : _middlewareData$autoP.index) || 0;
-                const currentPlacement = placements$12[currentIndex];
-                if (currentPlacement == null) {
-                    return {};
-                }
-                const alignmentSides = getAlignmentSides(currentPlacement, rects, await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating)));
-                if (placement !== currentPlacement) {
-                    return {
-                        reset: {
-                            placement: placements$12[0]
-                        }
-                    };
-                }
-                const currentOverflows = [overflow[getSide(currentPlacement)], overflow[alignmentSides[0]], overflow[alignmentSides[1]]];
-                const allOverflows = [...((_middlewareData$autoP2 = middlewareData.autoPlacement) == null ? void 0 : _middlewareData$autoP2.overflows) || [], {
-                    placement: currentPlacement,
-                    overflows: currentOverflows
-                }];
-                const nextPlacement = placements$12[currentIndex + 1];
-                if (nextPlacement) {
-                    return {
-                        data: {
-                            index: currentIndex + 1,
-                            overflows: allOverflows
-                        },
-                        reset: {
-                            placement: nextPlacement
-                        }
-                    };
-                }
-                const placementsSortedByMostSpace = allOverflows.map((d2) => {
-                    const alignment2 = getAlignment(d2.placement);
-                    return [d2.placement, alignment2 && crossAxis ? d2.overflows.slice(0, 2).reduce((acc, v3) => acc + v3, 0) : d2.overflows[0], d2.overflows];
-                }).sort((a2, b2) => a2[1] - b2[1]);
-                const placementsThatFitOnEachSide = placementsSortedByMostSpace.filter((d2) => d2[2].slice(
-                    0,
-                    getAlignment(d2[0]) ? 2 : 3
-                ).every((v3) => v3 <= 0));
-                const resetPlacement = ((_placementsThatFitOnE = placementsThatFitOnEachSide[0]) == null ? void 0 : _placementsThatFitOnE[0]) || placementsSortedByMostSpace[0][0];
-                if (resetPlacement !== placement) {
-                    return {
-                        data: {
-                            index: currentIndex + 1,
-                            overflows: allOverflows
-                        },
-                        reset: {
-                            placement: resetPlacement
-                        }
-                    };
-                }
-                return {};
-            }
-        };
-    };
-    const flip$1 = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            name: "flip",
-            options,
-            async fn(state) {
-                var _middlewareData$arrow, _middlewareData$flip;
-                const {
-                    placement,
-                    middlewareData,
-                    rects,
-                    initialPlacement,
-                    platform: platform2,
-                    elements
-                } = state;
-                const {
-                    mainAxis: checkMainAxis = true,
-                    crossAxis: checkCrossAxis = true,
-                    fallbackPlacements: specifiedFallbackPlacements,
-                    fallbackStrategy = "bestFit",
-                    fallbackAxisSideDirection = "none",
-                    flipAlignment = true,
-                    ...detectOverflowOptions
-                } = evaluate(options, state);
-                if ((_middlewareData$arrow = middlewareData.arrow) != null && _middlewareData$arrow.alignmentOffset) {
-                    return {};
-                }
-                const side = getSide(placement);
-                const isBasePlacement = getSide(initialPlacement) === initialPlacement;
-                const rtl = await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating));
-                const fallbackPlacements = specifiedFallbackPlacements || (isBasePlacement || !flipAlignment ? [getOppositePlacement(initialPlacement)] : getExpandedPlacements(initialPlacement));
-                if (!specifiedFallbackPlacements && fallbackAxisSideDirection !== "none") {
-                    fallbackPlacements.push(...getOppositeAxisPlacements(initialPlacement, flipAlignment, fallbackAxisSideDirection, rtl));
-                }
-                const placements2 = [initialPlacement, ...fallbackPlacements];
-                const overflow = await detectOverflow(state, detectOverflowOptions);
-                const overflows = [];
-                let overflowsData = ((_middlewareData$flip = middlewareData.flip) == null ? void 0 : _middlewareData$flip.overflows) || [];
-                if (checkMainAxis) {
-                    overflows.push(overflow[side]);
-                }
-                if (checkCrossAxis) {
-                    const sides2 = getAlignmentSides(placement, rects, rtl);
-                    overflows.push(overflow[sides2[0]], overflow[sides2[1]]);
-                }
-                overflowsData = [...overflowsData, {
-                    placement,
-                    overflows
-                }];
-                if (!overflows.every((side2) => side2 <= 0)) {
-                    var _middlewareData$flip2, _overflowsData$filter;
-                    const nextIndex = (((_middlewareData$flip2 = middlewareData.flip) == null ? void 0 : _middlewareData$flip2.index) || 0) + 1;
-                    const nextPlacement = placements2[nextIndex];
-                    if (nextPlacement) {
-                        return {
-                            data: {
-                                index: nextIndex,
-                                overflows: overflowsData
-                            },
-                            reset: {
-                                placement: nextPlacement
-                            }
-                        };
-                    }
-                    let resetPlacement = (_overflowsData$filter = overflowsData.filter((d2) => d2.overflows[0] <= 0).sort((a2, b2) => a2.overflows[1] - b2.overflows[1])[0]) == null ? void 0 : _overflowsData$filter.placement;
-                    if (!resetPlacement) {
-                        switch (fallbackStrategy) {
-                            case "bestFit": {
-                                var _overflowsData$map$so;
-                                const placement2 = (_overflowsData$map$so = overflowsData.map((d2) => [d2.placement, d2.overflows.filter((overflow2) => overflow2 > 0).reduce((acc, overflow2) => acc + overflow2, 0)]).sort((a2, b2) => a2[1] - b2[1])[0]) == null ? void 0 : _overflowsData$map$so[0];
-                                if (placement2) {
-                                    resetPlacement = placement2;
-                                }
-                                break;
-                            }
-                            case "initialPlacement":
-                                resetPlacement = initialPlacement;
-                                break;
-                        }
-                    }
-                    if (placement !== resetPlacement) {
-                        return {
-                            reset: {
-                                placement: resetPlacement
-                            }
-                        };
-                    }
-                }
-                return {};
-            }
-        };
-    };
-
-    function getSideOffsets(overflow, rect) {
-        return {
-            top: overflow.top - rect.height,
-            right: overflow.right - rect.width,
-            bottom: overflow.bottom - rect.height,
-            left: overflow.left - rect.width
-        };
-    }
-
-    function isAnySideFullyClipped(overflow) {
-        return sides.some((side) => overflow[side] >= 0);
-    }
-    const hide = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            name: "hide",
-            options,
-            async fn(state) {
-                const {
-                    rects
-                } = state;
-                const {
-                    strategy = "referenceHidden",
-                        ...detectOverflowOptions
-                } = evaluate(options, state);
-                switch (strategy) {
-                    case "referenceHidden": {
-                        const overflow = await detectOverflow(state, {
-                            ...detectOverflowOptions,
-                            elementContext: "reference"
-                        });
-                        const offsets = getSideOffsets(overflow, rects.reference);
-                        return {
-                            data: {
-                                referenceHiddenOffsets: offsets,
-                                referenceHidden: isAnySideFullyClipped(offsets)
-                            }
-                        };
-                    }
-                    case "escaped": {
-                        const overflow = await detectOverflow(state, {
-                            ...detectOverflowOptions,
-                            altBoundary: true
-                        });
-                        const offsets = getSideOffsets(overflow, rects.floating);
-                        return {
-                            data: {
-                                escapedOffsets: offsets,
-                                escaped: isAnySideFullyClipped(offsets)
-                            }
-                        };
-                    }
-                    default: {
-                        return {};
-                    }
-                }
-            }
-        };
-    };
-
-    function getBoundingRect(rects) {
-        const minX = min$1(...rects.map((rect) => rect.left));
-        const minY = min$1(...rects.map((rect) => rect.top));
-        const maxX = max$2(...rects.map((rect) => rect.right));
-        const maxY = max$2(...rects.map((rect) => rect.bottom));
-        return {
-            x: minX,
-            y: minY,
-            width: maxX - minX,
-            height: maxY - minY
-        };
-    }
-
-    function getRectsByLine(rects) {
-        const sortedRects = rects.slice().sort((a2, b2) => a2.y - b2.y);
-        const groups = [];
-        let prevRect = null;
-        for (let i2 = 0; i2 < sortedRects.length; i2++) {
-            const rect = sortedRects[i2];
-            if (!prevRect || rect.y - prevRect.y > prevRect.height / 2) {
-                groups.push([rect]);
-            } else {
-                groups[groups.length - 1].push(rect);
-            }
-            prevRect = rect;
-        }
-        return groups.map((rect) => rectToClientRect(getBoundingRect(rect)));
-    }
-    const inline = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            name: "inline",
-            options,
-            async fn(state) {
-                const {
-                    placement,
-                    elements,
-                    rects,
-                    platform: platform2,
-                    strategy
-                } = state;
-                const {
-                    padding = 2,
-                        x: x2,
-                        y: y2
-                } = evaluate(options, state);
-                const nativeClientRects = Array.from(await (platform2.getClientRects == null ? void 0 : platform2.getClientRects(elements.reference)) || []);
-                const clientRects = getRectsByLine(nativeClientRects);
-                const fallback = rectToClientRect(getBoundingRect(nativeClientRects));
-                const paddingObject = getPaddingObject(padding);
-
-                function getBoundingClientRect2() {
-                    if (clientRects.length === 2 && clientRects[0].left > clientRects[1].right && x2 != null && y2 != null) {
-                        return clientRects.find((rect) => x2 > rect.left - paddingObject.left && x2 < rect.right + paddingObject.right && y2 > rect.top - paddingObject.top && y2 < rect.bottom + paddingObject.bottom) || fallback;
-                    }
-                    if (clientRects.length >= 2) {
-                        if (getSideAxis(placement) === "y") {
-                            const firstRect = clientRects[0];
-                            const lastRect = clientRects[clientRects.length - 1];
-                            const isTop = getSide(placement) === "top";
-                            const top3 = firstRect.top;
-                            const bottom3 = lastRect.bottom;
-                            const left3 = isTop ? firstRect.left : lastRect.left;
-                            const right3 = isTop ? firstRect.right : lastRect.right;
-                            const width2 = right3 - left3;
-                            const height2 = bottom3 - top3;
-                            return {
-                                top: top3,
-                                bottom: bottom3,
-                                left: left3,
-                                right: right3,
-                                width: width2,
-                                height: height2,
-                                x: left3,
-                                y: top3
-                            };
-                        }
-                        const isLeftSide = getSide(placement) === "left";
-                        const maxRight = max$2(...clientRects.map((rect) => rect.right));
-                        const minLeft = min$1(...clientRects.map((rect) => rect.left));
-                        const measureRects = clientRects.filter((rect) => isLeftSide ? rect.left === minLeft : rect.right === maxRight);
-                        const top2 = measureRects[0].top;
-                        const bottom2 = measureRects[measureRects.length - 1].bottom;
-                        const left2 = minLeft;
-                        const right2 = maxRight;
-                        const width = right2 - left2;
-                        const height = bottom2 - top2;
-                        return {
-                            top: top2,
-                            bottom: bottom2,
-                            left: left2,
-                            right: right2,
-                            width,
-                            height,
-                            x: left2,
-                            y: top2
-                        };
-                    }
-                    return fallback;
-                }
-                const resetRects = await platform2.getElementRects({
-                    reference: {
-                        getBoundingClientRect: getBoundingClientRect2
-                    },
-                    floating: elements.floating,
-                    strategy
-                });
-                if (rects.reference.x !== resetRects.reference.x || rects.reference.y !== resetRects.reference.y || rects.reference.width !== resetRects.reference.width || rects.reference.height !== resetRects.reference.height) {
-                    return {
-                        reset: {
-                            rects: resetRects
-                        }
-                    };
-                }
-                return {};
-            }
-        };
-    };
-    const shift$2 = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            name: "shift",
-            options,
-            async fn(state) {
-                const {
-                    x: x2,
-                    y: y2,
-                    placement
-                } = state;
-                const {
-                    mainAxis: checkMainAxis = true,
-                    crossAxis: checkCrossAxis = false,
-                    limiter = {
-                        fn: (_ref2) => {
-                            let {
-                                x: x3,
-                                y: y3
-                            } = _ref2;
-                            return {
-                                x: x3,
-                                y: y3
-                            };
-                        }
-                    },
-                    ...detectOverflowOptions
-                } = evaluate(options, state);
-                const coords = {
-                    x: x2,
-                    y: y2
-                };
-                const overflow = await detectOverflow(state, detectOverflowOptions);
-                const crossAxis = getSideAxis(getSide(placement));
-                const mainAxis = getOppositeAxis(crossAxis);
-                let mainAxisCoord = coords[mainAxis];
-                let crossAxisCoord = coords[crossAxis];
-                if (checkMainAxis) {
-                    const minSide = mainAxis === "y" ? "top" : "left";
-                    const maxSide = mainAxis === "y" ? "bottom" : "right";
-                    const min2 = mainAxisCoord + overflow[minSide];
-                    const max2 = mainAxisCoord - overflow[maxSide];
-                    mainAxisCoord = clamp$1(min2, mainAxisCoord, max2);
-                }
-                if (checkCrossAxis) {
-                    const minSide = crossAxis === "y" ? "top" : "left";
-                    const maxSide = crossAxis === "y" ? "bottom" : "right";
-                    const min2 = crossAxisCoord + overflow[minSide];
-                    const max2 = crossAxisCoord - overflow[maxSide];
-                    crossAxisCoord = clamp$1(min2, crossAxisCoord, max2);
-                }
-                const limitedCoords = limiter.fn({
-                    ...state,
-                    [mainAxis]: mainAxisCoord,
-                    [crossAxis]: crossAxisCoord
-                });
-                return {
-                    ...limitedCoords,
-                    data: {
-                        x: limitedCoords.x - x2,
-                        y: limitedCoords.y - y2
-                    }
-                };
-            }
-        };
-    };
-    const limitShift = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            options,
-            fn(state) {
-                const {
-                    x: x2,
-                    y: y2,
-                    placement,
-                    rects,
-                    middlewareData
-                } = state;
-                const {
-                    offset: offset2 = 0,
-                    mainAxis: checkMainAxis = true,
-                    crossAxis: checkCrossAxis = true
-                } = evaluate(options, state);
-                const coords = {
-                    x: x2,
-                    y: y2
-                };
-                const crossAxis = getSideAxis(placement);
-                const mainAxis = getOppositeAxis(crossAxis);
-                let mainAxisCoord = coords[mainAxis];
-                let crossAxisCoord = coords[crossAxis];
-                const rawOffset = evaluate(offset2, state);
-                const computedOffset = typeof rawOffset === "number" ? {
-                    mainAxis: rawOffset,
-                    crossAxis: 0
-                } : {
-                    mainAxis: 0,
-                    crossAxis: 0,
-                    ...rawOffset
-                };
-                if (checkMainAxis) {
-                    const len = mainAxis === "y" ? "height" : "width";
-                    const limitMin = rects.reference[mainAxis] - rects.floating[len] + computedOffset.mainAxis;
-                    const limitMax = rects.reference[mainAxis] + rects.reference[len] - computedOffset.mainAxis;
-                    if (mainAxisCoord < limitMin) {
-                        mainAxisCoord = limitMin;
-                    } else if (mainAxisCoord > limitMax) {
-                        mainAxisCoord = limitMax;
-                    }
-                }
-                if (checkCrossAxis) {
-                    var _middlewareData$offse, _middlewareData$offse2;
-                    const len = mainAxis === "y" ? "width" : "height";
-                    const isOriginSide = ["top", "left"].includes(getSide(placement));
-                    const limitMin = rects.reference[crossAxis] - rects.floating[len] + (isOriginSide ? ((_middlewareData$offse = middlewareData.offset) == null ? void 0 : _middlewareData$offse[crossAxis]) || 0 : 0) + (isOriginSide ? 0 : computedOffset.crossAxis);
-                    const limitMax = rects.reference[crossAxis] + rects.reference[len] + (isOriginSide ? 0 : ((_middlewareData$offse2 = middlewareData.offset) == null ? void 0 : _middlewareData$offse2[crossAxis]) || 0) - (isOriginSide ? computedOffset.crossAxis : 0);
-                    if (crossAxisCoord < limitMin) {
-                        crossAxisCoord = limitMin;
-                    } else if (crossAxisCoord > limitMax) {
-                        crossAxisCoord = limitMax;
-                    }
-                }
-                return {
-                    [mainAxis]: mainAxisCoord,
-                    [crossAxis]: crossAxisCoord
-                };
-            }
-        };
-    };
-    const size$2 = function(options) {
-        if (options === void 0) {
-            options = {};
-        }
-        return {
-            name: "size",
-            options,
-            async fn(state) {
-                const {
-                    placement,
-                    rects,
-                    platform: platform2,
-                    elements
-                } = state;
-                const {
-                    apply = () => {},
-                        ...detectOverflowOptions
-                } = evaluate(options, state);
-                const overflow = await detectOverflow(state, detectOverflowOptions);
-                const side = getSide(placement);
-                const alignment = getAlignment(placement);
-                const isYAxis = getSideAxis(placement) === "y";
-                const {
-                    width,
-                    height
-                } = rects.floating;
-                let heightSide;
-                let widthSide;
-                if (side === "top" || side === "bottom") {
-                    heightSide = side;
-                    widthSide = alignment === (await (platform2.isRTL == null ? void 0 : platform2.isRTL(elements.floating)) ? "start" : "end") ? "left" : "right";
-                } else {
-                    widthSide = side;
-                    heightSide = alignment === "end" ? "top" : "bottom";
-                }
-                const overflowAvailableHeight = height - overflow[heightSide];
-                const overflowAvailableWidth = width - overflow[widthSide];
-                const noShift = !state.middlewareData.shift;
-                let availableHeight = overflowAvailableHeight;
-                let availableWidth = overflowAvailableWidth;
-                if (isYAxis) {
-                    const maximumClippingWidth = width - overflow.left - overflow.right;
-                    availableWidth = alignment || noShift ? min$1(overflowAvailableWidth, maximumClippingWidth) : maximumClippingWidth;
-                } else {
-                    const maximumClippingHeight = height - overflow.top - overflow.bottom;
-                    availableHeight = alignment || noShift ? min$1(overflowAvailableHeight, maximumClippingHeight) : maximumClippingHeight;
-                }
-                if (noShift && !alignment) {
-                    const xMin = max$2(overflow.left, 0);
-                    const xMax = max$2(overflow.right, 0);
-                    const yMin = max$2(overflow.top, 0);
-                    const yMax = max$2(overflow.bottom, 0);
-                    if (isYAxis) {
-                        availableWidth = width - 2 * (xMin !== 0 || xMax !== 0 ? xMin + xMax : max$2(overflow.left, overflow.right));
-                    } else {
-                        availableHeight = height - 2 * (yMin !== 0 || yMax !== 0 ? yMin + yMax : max$2(overflow.top, overflow.bottom));
-                    }
-                }
-                await apply({
-                    ...state,
-                    availableWidth,
-                    availableHeight
-                });
-                const nextDimensions = await platform2.getDimensions(elements.floating);
-                if (width !== nextDimensions.width || height !== nextDimensions.height) {
-                    return {
-                        reset: {
-                            rects: true
-                        }
-                    };
-                }
-                return {};
-            }
-        };
-    };
-
-    function getCssDimensions(element2) {
-        const css2 = getComputedStyle$1(element2);
-        let width = parseFloat(css2.width) || 0;
-        let height = parseFloat(css2.height) || 0;
-        const hasOffset = isHTMLElement(element2);
-        const offsetWidth = hasOffset ? element2.offsetWidth : width;
-        const offsetHeight = hasOffset ? element2.offsetHeight : height;
-        const shouldFallback = round$2(width) !== offsetWidth || round$2(height) !== offsetHeight;
-        if (shouldFallback) {
-            width = offsetWidth;
-            height = offsetHeight;
-        }
-        return {
-            width,
-            height,
-            $: shouldFallback
-        };
+                            return [2, items];
+                        }
+                        return [4, Promise.all(items.map(toFilePromises))];
+                    case 1:
+                        files = _a3.sent();
+                        return [2, noIgnoredFiles(flatten$1(files))];
+                    case 2:
+                        return [2, noIgnoredFiles(fromList(dt2.files).map(function(file) {
+                            return toFileWithPath(file);
+                        }))];
+                }
+            });
+        });
     }
 
-    function unwrapElement(element2) {
-        return !isElement$1(element2) ? element2.contextElement : element2;
+    function noIgnoredFiles(files) {
+        return files.filter(function(file) {
+            return FILES_TO_IGNORE.indexOf(file.name) === -1;
+        });
     }
 
-    function getScale$1(element2) {
-        const domElement2 = unwrapElement(element2);
-        if (!isHTMLElement(domElement2)) {
-            return createCoords(1);
+    function fromList(items) {
+        var files = [];
+        for (var i2 = 0; i2 < items.length; i2++) {
+            var file = items[i2];
+            files.push(file);
         }
-        const rect = domElement2.getBoundingClientRect();
-        const {
-            width,
-            height,
-            $: $2
-        } = getCssDimensions(domElement2);
-        let x2 = ($2 ? round$2(rect.width) : rect.width) / width;
-        let y2 = ($2 ? round$2(rect.height) : rect.height) / height;
-        if (!x2 || !Number.isFinite(x2)) {
-            x2 = 1;
+        return files;
+    }
+
+    function toFilePromises(item) {
+        if (typeof item.webkitGetAsEntry !== "function") {
+            return fromDataTransferItem(item);
         }
-        if (!y2 || !Number.isFinite(y2)) {
-            y2 = 1;
+        var entry = item.webkitGetAsEntry();
+        if (entry && entry.isDirectory) {
+            return fromDirEntry(entry);
         }
-        return {
-            x: x2,
-            y: y2
-        };
+        return fromDataTransferItem(item);
     }
-    const noOffsets = /* @__PURE__ */ createCoords(0);
 
-    function getVisualOffsets(element2) {
-        const win = getWindow(element2);
-        if (!isWebKit() || !win.visualViewport) {
-            return noOffsets;
-        }
-        return {
-            x: win.visualViewport.offsetLeft,
-            y: win.visualViewport.offsetTop
-        };
+    function flatten$1(items) {
+        return items.reduce(function(acc, files) {
+            return __spread(acc, Array.isArray(files) ? flatten$1(files) : [files]);
+        }, []);
     }
 
-    function shouldAddVisualOffsets(element2, isFixed, floatingOffsetParent) {
-        if (isFixed === void 0) {
-            isFixed = false;
-        }
-        if (!floatingOffsetParent || isFixed && floatingOffsetParent !== getWindow(element2)) {
-            return false;
+    function fromDataTransferItem(item) {
+        var file = item.getAsFile();
+        if (!file) {
+            return Promise.reject(item + " is not a File");
         }
-        return isFixed;
+        var fwp = toFileWithPath(file);
+        return Promise.resolve(fwp);
     }
 
-    function getBoundingClientRect(element2, includeScale, isFixedStrategy, offsetParent) {
-        if (includeScale === void 0) {
-            includeScale = false;
-        }
-        if (isFixedStrategy === void 0) {
-            isFixedStrategy = false;
-        }
-        const clientRect = element2.getBoundingClientRect();
-        const domElement2 = unwrapElement(element2);
-        let scale = createCoords(1);
-        if (includeScale) {
-            if (offsetParent) {
-                if (isElement$1(offsetParent)) {
-                    scale = getScale$1(offsetParent);
-                }
-            } else {
-                scale = getScale$1(element2);
-            }
-        }
-        const visualOffsets = shouldAddVisualOffsets(domElement2, isFixedStrategy, offsetParent) ? getVisualOffsets(domElement2) : createCoords(0);
-        let x2 = (clientRect.left + visualOffsets.x) / scale.x;
-        let y2 = (clientRect.top + visualOffsets.y) / scale.y;
-        let width = clientRect.width / scale.x;
-        let height = clientRect.height / scale.y;
-        if (domElement2) {
-            const win = getWindow(domElement2);
-            const offsetWin = offsetParent && isElement$1(offsetParent) ? getWindow(offsetParent) : offsetParent;
-            let currentWin = win;
-            let currentIFrame = currentWin.frameElement;
-            while (currentIFrame && offsetParent && offsetWin !== currentWin) {
-                const iframeScale = getScale$1(currentIFrame);
-                const iframeRect = currentIFrame.getBoundingClientRect();
-                const css2 = getComputedStyle$1(currentIFrame);
-                const left2 = iframeRect.left + (currentIFrame.clientLeft + parseFloat(css2.paddingLeft)) * iframeScale.x;
-                const top2 = iframeRect.top + (currentIFrame.clientTop + parseFloat(css2.paddingTop)) * iframeScale.y;
-                x2 *= iframeScale.x;
-                y2 *= iframeScale.y;
-                width *= iframeScale.x;
-                height *= iframeScale.y;
-                x2 += left2;
-                y2 += top2;
-                currentWin = getWindow(currentIFrame);
-                currentIFrame = currentWin.frameElement;
-            }
-        }
-        return rectToClientRect({
-            width,
-            height,
-            x: x2,
-            y: y2
+    function fromEntry(entry) {
+        return __awaiter$2(this, void 0, void 0, function() {
+            return __generator(this, function(_a3) {
+                return [2, entry.isDirectory ? fromDirEntry(entry) : fromFileEntry(entry)];
+            });
         });
     }
-    const topLayerSelectors = [":popover-open", ":modal"];
 
-    function isTopLayer(floating) {
-        return topLayerSelectors.some((selector2) => {
-            try {
-                return floating.matches(selector2);
-            } catch (e3) {
-                return false;
+    function fromDirEntry(entry) {
+        var reader = entry.createReader();
+        return new Promise(function(resolve2, reject) {
+            var entries = [];
+
+            function readEntries() {
+                var _this = this;
+                reader.readEntries(function(batch) {
+                    return __awaiter$2(_this, void 0, void 0, function() {
+                        var files, err_1, items;
+                        return __generator(this, function(_a3) {
+                            switch (_a3.label) {
+                                case 0:
+                                    if (!!batch.length)
+                                        return [3, 5];
+                                    _a3.label = 1;
+                                case 1:
+                                    _a3.trys.push([1, 3, , 4]);
+                                    return [4, Promise.all(entries)];
+                                case 2:
+                                    files = _a3.sent();
+                                    resolve2(files);
+                                    return [3, 4];
+                                case 3:
+                                    err_1 = _a3.sent();
+                                    reject(err_1);
+                                    return [3, 4];
+                                case 4:
+                                    return [3, 6];
+                                case 5:
+                                    items = Promise.all(batch.map(fromEntry));
+                                    entries.push(items);
+                                    readEntries();
+                                    _a3.label = 6;
+                                case 6:
+                                    return [2];
+                            }
+                        });
+                    });
+                }, function(err) {
+                    reject(err);
+                });
             }
+            readEntries();
         });
     }
 
-    function convertOffsetParentRelativeRectToViewportRelativeRect(_ref2) {
-        let {
-            elements,
-            rect,
-            offsetParent,
-            strategy
-        } = _ref2;
-        const isFixed = strategy === "fixed";
-        const documentElement = getDocumentElement(offsetParent);
-        const topLayer = elements ? isTopLayer(elements.floating) : false;
-        if (offsetParent === documentElement || topLayer && isFixed) {
-            return rect;
-        }
-        let scroll = {
-            scrollLeft: 0,
-            scrollTop: 0
-        };
-        let scale = createCoords(1);
-        const offsets = createCoords(0);
-        const isOffsetParentAnElement = isHTMLElement(offsetParent);
-        if (isOffsetParentAnElement || !isOffsetParentAnElement && !isFixed) {
-            if (getNodeName(offsetParent) !== "body" || isOverflowElement(documentElement)) {
-                scroll = getNodeScroll(offsetParent);
-            }
-            if (isHTMLElement(offsetParent)) {
-                const offsetRect = getBoundingClientRect(offsetParent);
-                scale = getScale$1(offsetParent);
-                offsets.x = offsetRect.x + offsetParent.clientLeft;
-                offsets.y = offsetRect.y + offsetParent.clientTop;
-            }
-        }
-        return {
-            width: rect.width * scale.x,
-            height: rect.height * scale.y,
-            x: rect.x * scale.x - scroll.scrollLeft * scale.x + offsets.x,
-            y: rect.y * scale.y - scroll.scrollTop * scale.y + offsets.y
-        };
+    function fromFileEntry(entry) {
+        return __awaiter$2(this, void 0, void 0, function() {
+            return __generator(this, function(_a3) {
+                return [2, new Promise(function(resolve2, reject) {
+                    entry.file(function(file) {
+                        var fwp = toFileWithPath(file, entry.fullPath);
+                        resolve2(fwp);
+                    }, function(err) {
+                        reject(err);
+                    });
+                })];
+            });
+        });
     }
+    var _default$1 = function(file, acceptedFiles) {
+        if (file && acceptedFiles) {
+            var acceptedFilesArray = Array.isArray(acceptedFiles) ? acceptedFiles : acceptedFiles.split(",");
+            var fileName = file.name || "";
+            var mimeType = (file.type || "").toLowerCase();
+            var baseMimeType = mimeType.replace(/\/.*$/, "");
+            return acceptedFilesArray.some(function(type2) {
+                var validType = type2.trim().toLowerCase();
+                if (validType.charAt(0) === ".") {
+                    return fileName.toLowerCase().endsWith(validType);
+                } else if (validType.endsWith("/*")) {
+                    return baseMimeType === validType.replace(/\/.*$/, "");
+                }
+                return mimeType === validType;
+            });
+        }
+        return true;
+    };
 
-    function getClientRects(element2) {
-        return Array.from(element2.getClientRects());
+    function _slicedToArray$9(arr, i2) {
+        return _arrayWithHoles$9(arr) || _iterableToArrayLimit$9(arr, i2) || _nonIterableRest$9();
     }
 
-    function getWindowScrollBarX(element2) {
-        return getBoundingClientRect(getDocumentElement(element2)).left + getNodeScroll(element2).scrollLeft;
+    function _nonIterableRest$9() {
+        throw new TypeError("Invalid attempt to destructure non-iterable instance");
     }
 
-    function getDocumentRect(element2) {
-        const html2 = getDocumentElement(element2);
-        const scroll = getNodeScroll(element2);
-        const body = element2.ownerDocument.body;
-        const width = max$2(html2.scrollWidth, html2.clientWidth, body.scrollWidth, body.clientWidth);
-        const height = max$2(html2.scrollHeight, html2.clientHeight, body.scrollHeight, body.clientHeight);
-        let x2 = -scroll.scrollLeft + getWindowScrollBarX(element2);
-        const y2 = -scroll.scrollTop;
-        if (getComputedStyle$1(body).direction === "rtl") {
-            x2 += max$2(html2.clientWidth, body.clientWidth) - width;
+    function _iterableToArrayLimit$9(arr, i2) {
+        if (!(Symbol.iterator in Object(arr) || Object.prototype.toString.call(arr) === "[object Arguments]")) {
+            return;
         }
-        return {
-            width,
-            height,
-            x: x2,
-            y: y2
-        };
-    }
-
-    function getViewportRect(element2, strategy) {
-        const win = getWindow(element2);
-        const html2 = getDocumentElement(element2);
-        const visualViewport = win.visualViewport;
-        let width = html2.clientWidth;
-        let height = html2.clientHeight;
-        let x2 = 0;
-        let y2 = 0;
-        if (visualViewport) {
-            width = visualViewport.width;
-            height = visualViewport.height;
-            const visualViewportBased = isWebKit();
-            if (!visualViewportBased || visualViewportBased && strategy === "fixed") {
-                x2 = visualViewport.offsetLeft;
-                y2 = visualViewport.offsetTop;
+        var _arr = [];
+        var _n2 = true;
+        var _d = false;
+        var _e2 = void 0;
+        try {
+            for (var _i2 = arr[Symbol.iterator](), _s; !(_n2 = (_s = _i2.next()).done); _n2 = true) {
+                _arr.push(_s.value);
+                if (i2 && _arr.length === i2)
+                    break;
+            }
+        } catch (err) {
+            _d = true;
+            _e2 = err;
+        } finally {
+            try {
+                if (!_n2 && _i2["return"] != null)
+                    _i2["return"]();
+            } finally {
+                if (_d)
+                    throw _e2;
             }
         }
-        return {
-            width,
-            height,
-            x: x2,
-            y: y2
-        };
+        return _arr;
     }
 
-    function getInnerBoundingClientRect(element2, strategy) {
-        const clientRect = getBoundingClientRect(element2, true, strategy === "fixed");
-        const top2 = clientRect.top + element2.clientTop;
-        const left2 = clientRect.left + element2.clientLeft;
-        const scale = isHTMLElement(element2) ? getScale$1(element2) : createCoords(1);
-        const width = element2.clientWidth * scale.x;
-        const height = element2.clientHeight * scale.y;
-        const x2 = left2 * scale.x;
-        const y2 = top2 * scale.y;
+    function _arrayWithHoles$9(arr) {
+        if (Array.isArray(arr))
+            return arr;
+    }
+    var FILE_INVALID_TYPE = "file-invalid-type";
+    var FILE_TOO_LARGE = "file-too-large";
+    var FILE_TOO_SMALL = "file-too-small";
+    var TOO_MANY_FILES = "too-many-files";
+    var getInvalidTypeRejectionErr = function getInvalidTypeRejectionErr2(accept) {
+        accept = Array.isArray(accept) && accept.length === 1 ? accept[0] : accept;
+        var messageSuffix = Array.isArray(accept) ? "one of ".concat(accept.join(", ")) : accept;
         return {
-            width,
-            height,
-            x: x2,
-            y: y2
+            code: FILE_INVALID_TYPE,
+            message: "File type must be ".concat(messageSuffix)
+        };
+    };
+    var getTooLargeRejectionErr = function getTooLargeRejectionErr2(maxSize) {
+        return {
+            code: FILE_TOO_LARGE,
+            message: "File is larger than ".concat(maxSize, " bytes")
         };
+    };
+    var getTooSmallRejectionErr = function getTooSmallRejectionErr2(minSize) {
+        return {
+            code: FILE_TOO_SMALL,
+            message: "File is smaller than ".concat(minSize, " bytes")
+        };
+    };
+    var TOO_MANY_FILES_REJECTION = {
+        code: TOO_MANY_FILES,
+        message: "Too many files"
+    };
+
+    function fileAccepted(file, accept) {
+        var isAcceptable = file.type === "application/x-moz-file" || _default$1(file, accept);
+        return [isAcceptable, isAcceptable ? null : getInvalidTypeRejectionErr(accept)];
     }
 
-    function getClientRectFromClippingAncestor(element2, clippingAncestor, strategy) {
-        let rect;
-        if (clippingAncestor === "viewport") {
-            rect = getViewportRect(element2, strategy);
-        } else if (clippingAncestor === "document") {
-            rect = getDocumentRect(getDocumentElement(element2));
-        } else if (isElement$1(clippingAncestor)) {
-            rect = getInnerBoundingClientRect(clippingAncestor, strategy);
-        } else {
-            const visualOffsets = getVisualOffsets(element2);
-            rect = {
-                ...clippingAncestor,
-                x: clippingAncestor.x - visualOffsets.x,
-                y: clippingAncestor.y - visualOffsets.y
-            };
+    function fileMatchSize(file, minSize, maxSize) {
+        if (isDefined(file.size)) {
+            if (isDefined(minSize) && isDefined(maxSize)) {
+                if (file.size > maxSize)
+                    return [false, getTooLargeRejectionErr(maxSize)];
+                if (file.size < minSize)
+                    return [false, getTooSmallRejectionErr(minSize)];
+            } else if (isDefined(minSize) && file.size < minSize)
+                return [false, getTooSmallRejectionErr(minSize)];
+            else if (isDefined(maxSize) && file.size > maxSize)
+                return [false, getTooLargeRejectionErr(maxSize)];
         }
-        return rectToClientRect(rect);
+        return [true, null];
     }
 
-    function hasFixedPositionAncestor(element2, stopNode) {
-        const parentNode = getParentNode(element2);
-        if (parentNode === stopNode || !isElement$1(parentNode) || isLastTraversableNode(parentNode)) {
+    function isDefined(value) {
+        return value !== void 0 && value !== null;
+    }
+
+    function allFilesAccepted(_ref2) {
+        var files = _ref2.files,
+            accept = _ref2.accept,
+            minSize = _ref2.minSize,
+            maxSize = _ref2.maxSize,
+            multiple = _ref2.multiple;
+        if (!multiple && files.length > 1) {
             return false;
         }
-        return getComputedStyle$1(parentNode).position === "fixed" || hasFixedPositionAncestor(parentNode, stopNode);
+        return files.every(function(file) {
+            var _fileAccepted = fileAccepted(file, accept),
+                _fileAccepted2 = _slicedToArray$9(_fileAccepted, 1),
+                accepted = _fileAccepted2[0];
+            var _fileMatchSize = fileMatchSize(file, minSize, maxSize),
+                _fileMatchSize2 = _slicedToArray$9(_fileMatchSize, 1),
+                sizeMatch = _fileMatchSize2[0];
+            return accepted && sizeMatch;
+        });
     }
 
-    function getClippingElementAncestors(element2, cache2) {
-        const cachedResult = cache2.get(element2);
-        if (cachedResult) {
-            return cachedResult;
+    function isPropagationStopped(event2) {
+        if (typeof event2.isPropagationStopped === "function") {
+            return event2.isPropagationStopped();
+        } else if (typeof event2.cancelBubble !== "undefined") {
+            return event2.cancelBubble;
         }
-        let result = getOverflowAncestors(element2, [], false).filter((el) => isElement$1(el) && getNodeName(el) !== "body");
-        let currentContainingBlockComputedStyle = null;
-        const elementIsFixed = getComputedStyle$1(element2).position === "fixed";
-        let currentNode = elementIsFixed ? getParentNode(element2) : element2;
-        while (isElement$1(currentNode) && !isLastTraversableNode(currentNode)) {
-            const computedStyle = getComputedStyle$1(currentNode);
-            const currentNodeIsContaining = isContainingBlock(currentNode);
-            if (!currentNodeIsContaining && computedStyle.position === "fixed") {
-                currentContainingBlockComputedStyle = null;
-            }
-            const shouldDropCurrentNode = elementIsFixed ? !currentNodeIsContaining && !currentContainingBlockComputedStyle : !currentNodeIsContaining && computedStyle.position === "static" && !!currentContainingBlockComputedStyle && ["absolute", "fixed"].includes(currentContainingBlockComputedStyle.position) || isOverflowElement(currentNode) && !currentNodeIsContaining && hasFixedPositionAncestor(element2, currentNode);
-            if (shouldDropCurrentNode) {
-                result = result.filter((ancestor) => ancestor !== currentNode);
-            } else {
-                currentContainingBlockComputedStyle = computedStyle;
-            }
-            currentNode = getParentNode(currentNode);
+        return false;
+    }
+
+    function isEvtWithFiles(event2) {
+        if (!event2.dataTransfer) {
+            return !!event2.target && !!event2.target.files;
         }
-        cache2.set(element2, result);
-        return result;
+        return Array.prototype.some.call(event2.dataTransfer.types, function(type2) {
+            return type2 === "Files" || type2 === "application/x-moz-file";
+        });
     }
 
-    function getClippingRect(_ref2) {
-        let {
-            element: element2,
-            boundary,
-            rootBoundary,
-            strategy
-        } = _ref2;
-        const elementClippingAncestors = boundary === "clippingAncestors" ? getClippingElementAncestors(element2, this._c) : [].concat(boundary);
-        const clippingAncestors = [...elementClippingAncestors, rootBoundary];
-        const firstClippingAncestor = clippingAncestors[0];
-        const clippingRect = clippingAncestors.reduce((accRect, clippingAncestor) => {
-            const rect = getClientRectFromClippingAncestor(element2, clippingAncestor, strategy);
-            accRect.top = max$2(rect.top, accRect.top);
-            accRect.right = min$1(rect.right, accRect.right);
-            accRect.bottom = min$1(rect.bottom, accRect.bottom);
-            accRect.left = max$2(rect.left, accRect.left);
-            return accRect;
-        }, getClientRectFromClippingAncestor(element2, firstClippingAncestor, strategy));
-        return {
-            width: clippingRect.right - clippingRect.left,
-            height: clippingRect.bottom - clippingRect.top,
-            x: clippingRect.left,
-            y: clippingRect.top
-        };
+    function onDocumentDragOver(event2) {
+        event2.preventDefault();
     }
 
-    function getDimensions(element2) {
-        const {
-            width,
-            height
-        } = getCssDimensions(element2);
-        return {
-            width,
-            height
-        };
+    function isIe(userAgent2) {
+        return userAgent2.indexOf("MSIE") !== -1 || userAgent2.indexOf("Trident/") !== -1;
     }
 
-    function getRectRelativeToOffsetParent(element2, offsetParent, strategy) {
-        const isOffsetParentAnElement = isHTMLElement(offsetParent);
-        const documentElement = getDocumentElement(offsetParent);
-        const isFixed = strategy === "fixed";
-        const rect = getBoundingClientRect(element2, true, isFixed, offsetParent);
-        let scroll = {
-            scrollLeft: 0,
-            scrollTop: 0
-        };
-        const offsets = createCoords(0);
-        if (isOffsetParentAnElement || !isOffsetParentAnElement && !isFixed) {
-            if (getNodeName(offsetParent) !== "body" || isOverflowElement(documentElement)) {
-                scroll = getNodeScroll(offsetParent);
-            }
-            if (isOffsetParentAnElement) {
-                const offsetRect = getBoundingClientRect(offsetParent, true, isFixed, offsetParent);
-                offsets.x = offsetRect.x + offsetParent.clientLeft;
-                offsets.y = offsetRect.y + offsetParent.clientTop;
-            } else if (documentElement) {
-                offsets.x = getWindowScrollBarX(documentElement);
-            }
-        }
-        const x2 = rect.left + scroll.scrollLeft - offsets.x;
-        const y2 = rect.top + scroll.scrollTop - offsets.y;
-        return {
-            x: x2,
-            y: y2,
-            width: rect.width,
-            height: rect.height
-        };
+    function isEdge(userAgent2) {
+        return userAgent2.indexOf("Edge/") !== -1;
     }
 
-    function getTrueOffsetParent(element2, polyfill) {
-        if (!isHTMLElement(element2) || getComputedStyle$1(element2).position === "fixed") {
-            return null;
-        }
-        if (polyfill) {
-            return polyfill(element2);
-        }
-        return element2.offsetParent;
+    function isIeOrEdge() {
+        var userAgent2 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : window.navigator.userAgent;
+        return isIe(userAgent2) || isEdge(userAgent2);
     }
 
-    function getOffsetParent(element2, polyfill) {
-        const window2 = getWindow(element2);
-        if (!isHTMLElement(element2) || isTopLayer(element2)) {
-            return window2;
-        }
-        let offsetParent = getTrueOffsetParent(element2, polyfill);
-        while (offsetParent && isTableElement(offsetParent) && getComputedStyle$1(offsetParent).position === "static") {
-            offsetParent = getTrueOffsetParent(offsetParent, polyfill);
-        }
-        if (offsetParent && (getNodeName(offsetParent) === "html" || getNodeName(offsetParent) === "body" && getComputedStyle$1(offsetParent).position === "static" && !isContainingBlock(offsetParent))) {
-            return window2;
+    function composeEventHandlers() {
+        for (var _len = arguments.length, fns = new Array(_len), _key = 0; _key < _len; _key++) {
+            fns[_key] = arguments[_key];
         }
-        return offsetParent || getContainingBlock(element2) || window2;
-    }
-    const getElementRects = async function(data2) {
-        const getOffsetParentFn = this.getOffsetParent || getOffsetParent;
-        const getDimensionsFn = this.getDimensions;
-        return {
-            reference: getRectRelativeToOffsetParent(data2.reference, await getOffsetParentFn(data2.floating), data2.strategy),
-            floating: {
-                x: 0,
-                y: 0,
-                ...await getDimensionsFn(data2.floating)
+        return function(event2) {
+            for (var _len2 = arguments.length, args = new Array(_len2 > 1 ? _len2 - 1 : 0), _key2 = 1; _key2 < _len2; _key2++) {
+                args[_key2 - 1] = arguments[_key2];
             }
+            return fns.some(function(fn2) {
+                if (!isPropagationStopped(event2) && fn2) {
+                    fn2.apply(void 0, [event2].concat(args));
+                }
+                return isPropagationStopped(event2);
+            });
         };
-    };
+    }
 
-    function isRTL(element2) {
-        return getComputedStyle$1(element2).direction === "rtl";
+    function _toConsumableArray$2(arr) {
+        return _arrayWithoutHoles$2(arr) || _iterableToArray$2(arr) || _nonIterableSpread$2();
     }
-    const platform = {
-        convertOffsetParentRelativeRectToViewportRelativeRect,
-        getDocumentElement,
-        getClippingRect,
-        getOffsetParent,
-        getElementRects,
-        getClientRects,
-        getDimensions,
-        getScale: getScale$1,
-        isElement: isElement$1,
-        isRTL
-    };
 
-    function observeMove(element2, onMove) {
-        let io2 = null;
-        let timeoutId;
-        const root2 = getDocumentElement(element2);
+    function _nonIterableSpread$2() {
+        throw new TypeError("Invalid attempt to spread non-iterable instance");
+    }
 
-        function cleanup() {
-            var _io;
-            clearTimeout(timeoutId);
-            (_io = io2) == null || _io.disconnect();
-            io2 = null;
-        }
+    function _iterableToArray$2(iter2) {
+        if (Symbol.iterator in Object(iter2) || Object.prototype.toString.call(iter2) === "[object Arguments]")
+            return Array.from(iter2);
+    }
 
-        function refresh(skip, threshold) {
-            if (skip === void 0) {
-                skip = false;
-            }
-            if (threshold === void 0) {
-                threshold = 1;
-            }
-            cleanup();
-            const {
-                left: left2,
-                top: top2,
-                width,
-                height
-            } = element2.getBoundingClientRect();
-            if (!skip) {
-                onMove();
-            }
-            if (!width || !height) {
-                return;
+    function _arrayWithoutHoles$2(arr) {
+        if (Array.isArray(arr)) {
+            for (var i2 = 0, arr2 = new Array(arr.length); i2 < arr.length; i2++) {
+                arr2[i2] = arr[i2];
             }
-            const insetTop = floor(top2);
-            const insetRight = floor(root2.clientWidth - (left2 + width));
-            const insetBottom = floor(root2.clientHeight - (top2 + height));
-            const insetLeft = floor(left2);
-            const rootMargin = -insetTop + "px " + -insetRight + "px " + -insetBottom + "px " + -insetLeft + "px";
-            const options = {
-                rootMargin,
-                threshold: max$2(0, min$1(1, threshold)) || 1
-            };
-            let isFirstUpdate = true;
+            return arr2;
+        }
+    }
 
-            function handleObserve(entries) {
-                const ratio = entries[0].intersectionRatio;
-                if (ratio !== threshold) {
-                    if (!isFirstUpdate) {
-                        return refresh();
-                    }
-                    if (!ratio) {
-                        timeoutId = setTimeout(() => {
-                            refresh(false, 1e-7);
-                        }, 100);
-                    } else {
-                        refresh(false, ratio);
-                    }
-                }
-                isFirstUpdate = false;
+    function _slicedToArray$8(arr, i2) {
+        return _arrayWithHoles$8(arr) || _iterableToArrayLimit$8(arr, i2) || _nonIterableRest$8();
+    }
+
+    function _nonIterableRest$8() {
+        throw new TypeError("Invalid attempt to destructure non-iterable instance");
+    }
+
+    function _iterableToArrayLimit$8(arr, i2) {
+        if (!(Symbol.iterator in Object(arr) || Object.prototype.toString.call(arr) === "[object Arguments]")) {
+            return;
+        }
+        var _arr = [];
+        var _n2 = true;
+        var _d = false;
+        var _e2 = void 0;
+        try {
+            for (var _i2 = arr[Symbol.iterator](), _s; !(_n2 = (_s = _i2.next()).done); _n2 = true) {
+                _arr.push(_s.value);
+                if (i2 && _arr.length === i2)
+                    break;
             }
+        } catch (err) {
+            _d = true;
+            _e2 = err;
+        } finally {
             try {
-                io2 = new IntersectionObserver(handleObserve, {
-                    ...options,
-                    root: root2.ownerDocument
-                });
-            } catch (e3) {
-                io2 = new IntersectionObserver(handleObserve, options);
+                if (!_n2 && _i2["return"] != null)
+                    _i2["return"]();
+            } finally {
+                if (_d)
+                    throw _e2;
             }
-            io2.observe(element2);
         }
-        refresh(true);
-        return cleanup;
+        return _arr;
     }
 
-    function autoUpdate(reference2, floating, update2, options) {
-        if (options === void 0) {
-            options = {};
-        }
-        const {
-            ancestorScroll = true,
-                ancestorResize = true,
-                elementResize = typeof ResizeObserver === "function",
-                layoutShift = typeof IntersectionObserver === "function",
-                animationFrame = false
-        } = options;
-        const referenceEl = unwrapElement(reference2);
-        const ancestors = ancestorScroll || ancestorResize ? [...referenceEl ? getOverflowAncestors(referenceEl) : [], ...getOverflowAncestors(floating)] : [];
-        ancestors.forEach((ancestor) => {
-            ancestorScroll && ancestor.addEventListener("scroll", update2, {
-                passive: true
-            });
-            ancestorResize && ancestor.addEventListener("resize", update2);
-        });
-        const cleanupIo = referenceEl && layoutShift ? observeMove(referenceEl, update2) : null;
-        let reobserveFrame = -1;
-        let resizeObserver = null;
-        if (elementResize) {
-            resizeObserver = new ResizeObserver((_ref2) => {
-                let [firstEntry] = _ref2;
-                if (firstEntry && firstEntry.target === referenceEl && resizeObserver) {
-                    resizeObserver.unobserve(floating);
-                    cancelAnimationFrame(reobserveFrame);
-                    reobserveFrame = requestAnimationFrame(() => {
-                        var _resizeObserver;
-                        (_resizeObserver = resizeObserver) == null || _resizeObserver.observe(floating);
-                    });
-                }
-                update2();
-            });
-            if (referenceEl && !animationFrame) {
-                resizeObserver.observe(referenceEl);
-            }
-            resizeObserver.observe(floating);
-        }
-        let frameId;
-        let prevRefRect = animationFrame ? getBoundingClientRect(reference2) : null;
-        if (animationFrame) {
-            frameLoop();
-        }
+    function _arrayWithHoles$8(arr) {
+        if (Array.isArray(arr))
+            return arr;
+    }
 
-        function frameLoop() {
-            const nextRefRect = getBoundingClientRect(reference2);
-            if (prevRefRect && (nextRefRect.x !== prevRefRect.x || nextRefRect.y !== prevRefRect.y || nextRefRect.width !== prevRefRect.width || nextRefRect.height !== prevRefRect.height)) {
-                update2();
-            }
-            prevRefRect = nextRefRect;
-            frameId = requestAnimationFrame(frameLoop);
+    function ownKeys$6(object2, enumerableOnly) {
+        var keys2 = Object.keys(object2);
+        if (Object.getOwnPropertySymbols) {
+            var symbols = Object.getOwnPropertySymbols(object2);
+            if (enumerableOnly)
+                symbols = symbols.filter(function(sym) {
+                    return Object.getOwnPropertyDescriptor(object2, sym).enumerable;
+                });
+            keys2.push.apply(keys2, symbols);
         }
-        update2();
-        return () => {
-            var _resizeObserver2;
-            ancestors.forEach((ancestor) => {
-                ancestorScroll && ancestor.removeEventListener("scroll", update2);
-                ancestorResize && ancestor.removeEventListener("resize", update2);
-            });
-            cleanupIo == null || cleanupIo();
-            (_resizeObserver2 = resizeObserver) == null || _resizeObserver2.disconnect();
-            resizeObserver = null;
-            if (animationFrame) {
-                cancelAnimationFrame(frameId);
-            }
-        };
+        return keys2;
     }
-    autoPlacement;
-    const shift$1 = shift$2;
-    const flip = flip$1;
-    const size$1 = size$2;
-    hide;
-    arrow;
-    inline;
-    limitShift;
-    const computePosition = (reference2, floating, options) => {
-        const cache2 = /* @__PURE__ */ new Map();
-        const mergedOptions = {
-            platform,
-            ...options
-        };
-        const platformWithCache = {
-            ...mergedOptions.platform,
-            _c: cache2
-        };
-        return computePosition$1(reference2, floating, {
-            ...mergedOptions,
-            platform: platformWithCache
-        });
-    };
-    var index$3 = typeof document !== "undefined" ? React.useLayoutEffect : React.useEffect;
 
-    function deepEqual(a2, b2) {
-        if (a2 === b2) {
-            return true;
-        }
-        if (typeof a2 !== typeof b2) {
-            return false;
-        }
-        if (typeof a2 === "function" && a2.toString() === b2.toString()) {
-            return true;
-        }
-        let length;
-        let i2;
-        let keys2;
-        if (a2 && b2 && typeof a2 === "object") {
-            if (Array.isArray(a2)) {
-                length = a2.length;
-                if (length !== b2.length)
-                    return false;
-                for (i2 = length; i2-- !== 0;) {
-                    if (!deepEqual(a2[i2], b2[i2])) {
-                        return false;
-                    }
-                }
-                return true;
-            }
-            keys2 = Object.keys(a2);
-            length = keys2.length;
-            if (length !== Object.keys(b2).length) {
-                return false;
-            }
-            for (i2 = length; i2-- !== 0;) {
-                if (!{}.hasOwnProperty.call(b2, keys2[i2])) {
-                    return false;
-                }
-            }
-            for (i2 = length; i2-- !== 0;) {
-                const key = keys2[i2];
-                if (key === "_owner" && a2.$$typeof) {
-                    continue;
-                }
-                if (!deepEqual(a2[key], b2[key])) {
-                    return false;
-                }
+    function _objectSpread$5(target) {
+        for (var i2 = 1; i2 < arguments.length; i2++) {
+            var source = arguments[i2] != null ? arguments[i2] : {};
+            if (i2 % 2) {
+                ownKeys$6(source, true).forEach(function(key) {
+                    _defineProperty$n(target, key, source[key]);
+                });
+            } else if (Object.getOwnPropertyDescriptors) {
+                Object.defineProperties(target, Object.getOwnPropertyDescriptors(source));
+            } else {
+                ownKeys$6(source).forEach(function(key) {
+                    Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));
+                });
             }
-            return true;
         }
-        return a2 !== a2 && b2 !== b2;
+        return target;
     }
 
-    function getDPR(element2) {
-        if (typeof window === "undefined") {
-            return 1;
+    function _defineProperty$n(obj, key, value) {
+        if (key in obj) {
+            Object.defineProperty(obj, key, {
+                value,
+                enumerable: true,
+                configurable: true,
+                writable: true
+            });
+        } else {
+            obj[key] = value;
         }
-        const win = element2.ownerDocument.defaultView || window;
-        return win.devicePixelRatio || 1;
-    }
-
-    function roundByDPR(element2, value) {
-        const dpr = getDPR(element2);
-        return Math.round(value * dpr) / dpr;
+        return obj;
     }
 
-    function useLatestRef(value) {
-        const ref2 = React__namespace.useRef(value);
-        index$3(() => {
-            ref2.current = value;
-        });
-        return ref2;
+    function _objectWithoutProperties$1(source, excluded) {
+        if (source == null)
+            return {};
+        var target = _objectWithoutPropertiesLoose$2(source, excluded);
+        var key, i2;
+        if (Object.getOwnPropertySymbols) {
+            var sourceSymbolKeys = Object.getOwnPropertySymbols(source);
+            for (i2 = 0; i2 < sourceSymbolKeys.length; i2++) {
+                key = sourceSymbolKeys[i2];
+                if (excluded.indexOf(key) >= 0)
+                    continue;
+                if (!Object.prototype.propertyIsEnumerable.call(source, key))
+                    continue;
+                target[key] = source[key];
+            }
+        }
+        return target;
     }
 
-    function useFloating$1(options) {
-        if (options === void 0) {
-            options = {};
+    function _objectWithoutPropertiesLoose$2(source, excluded) {
+        if (source == null)
+            return {};
+        var target = {};
+        var sourceKeys = Object.keys(source);
+        var key, i2;
+        for (i2 = 0; i2 < sourceKeys.length; i2++) {
+            key = sourceKeys[i2];
+            if (excluded.indexOf(key) >= 0)
+                continue;
+            target[key] = source[key];
         }
-        const {
-            placement = "bottom",
-                strategy = "absolute",
-                middleware = [],
-                platform: platform2,
-                elements: {
-                    reference: externalReference,
-                    floating: externalFloating
-                } = {},
-                transform = true,
-                whileElementsMounted,
+        return target;
+    }
+    var Dropzone$1 = React.forwardRef(function(_ref2, ref2) {
+        var children2 = _ref2.children,
+            params = _objectWithoutProperties$1(_ref2, ["children"]);
+        var _useDropzone = useDropzone(params),
+            open = _useDropzone.open,
+            props = _objectWithoutProperties$1(_useDropzone, ["open"]);
+        React.useImperativeHandle(ref2, function() {
+            return {
                 open
-        } = options;
-        const [data2, setData] = React__namespace.useState({
-            x: 0,
-            y: 0,
-            strategy,
-            placement,
-            middlewareData: {},
-            isPositioned: false
-        });
-        const [latestMiddleware, setLatestMiddleware] = React__namespace.useState(middleware);
-        if (!deepEqual(latestMiddleware, middleware)) {
-            setLatestMiddleware(middleware);
-        }
-        const [_reference, _setReference] = React__namespace.useState(null);
-        const [_floating, _setFloating] = React__namespace.useState(null);
-        const setReference = React__namespace.useCallback((node2) => {
-            if (node2 !== referenceRef.current) {
-                referenceRef.current = node2;
-                _setReference(node2);
-            }
-        }, []);
-        const setFloating = React__namespace.useCallback((node2) => {
-            if (node2 !== floatingRef.current) {
-                floatingRef.current = node2;
-                _setFloating(node2);
-            }
-        }, []);
-        const referenceEl = externalReference || _reference;
-        const floatingEl = externalFloating || _floating;
-        const referenceRef = React__namespace.useRef(null);
-        const floatingRef = React__namespace.useRef(null);
-        const dataRef = React__namespace.useRef(data2);
-        const hasWhileElementsMounted = whileElementsMounted != null;
-        const whileElementsMountedRef = useLatestRef(whileElementsMounted);
-        const platformRef = useLatestRef(platform2);
-        const update2 = React__namespace.useCallback(() => {
-            if (!referenceRef.current || !floatingRef.current) {
-                return;
-            }
-            const config2 = {
-                placement,
-                strategy,
-                middleware: latestMiddleware
             };
-            if (platformRef.current) {
-                config2.platform = platformRef.current;
-            }
-            computePosition(referenceRef.current, floatingRef.current, config2).then((data3) => {
-                const fullData = {
-                    ...data3,
-                    isPositioned: true
-                };
-                if (isMountedRef.current && !deepEqual(dataRef.current, fullData)) {
-                    dataRef.current = fullData;
-                    ReactDOM__namespace.flushSync(() => {
-                        setData(fullData);
-                    });
-                }
-            });
-        }, [latestMiddleware, placement, strategy, platformRef]);
-        index$3(() => {
-            if (open === false && dataRef.current.isPositioned) {
-                dataRef.current.isPositioned = false;
-                setData((data3) => ({
-                    ...data3,
-                    isPositioned: false
-                }));
-            }
         }, [open]);
-        const isMountedRef = React__namespace.useRef(false);
-        index$3(() => {
-            isMountedRef.current = true;
-            return () => {
-                isMountedRef.current = false;
-            };
-        }, []);
-        index$3(() => {
-            if (referenceEl)
-                referenceRef.current = referenceEl;
-            if (floatingEl)
-                floatingRef.current = floatingEl;
-            if (referenceEl && floatingEl) {
-                if (whileElementsMountedRef.current) {
-                    return whileElementsMountedRef.current(referenceEl, floatingEl, update2);
-                }
-                update2();
-            }
-        }, [referenceEl, floatingEl, update2, whileElementsMountedRef, hasWhileElementsMounted]);
-        const refs = React__namespace.useMemo(() => ({
-            reference: referenceRef,
-            floating: floatingRef,
-            setReference,
-            setFloating
-        }), [setReference, setFloating]);
-        const elements = React__namespace.useMemo(() => ({
-            reference: referenceEl,
-            floating: floatingEl
-        }), [referenceEl, floatingEl]);
-        const floatingStyles = React__namespace.useMemo(() => {
-            const initialStyles = {
-                position: strategy,
-                left: 0,
-                top: 0
-            };
-            if (!elements.floating) {
-                return initialStyles;
+        return React__default.default.createElement(React.Fragment, null, children2(_objectSpread$5({}, props, {
+            open
+        })));
+    });
+    Dropzone$1.displayName = "Dropzone";
+    Dropzone$1.propTypes = {
+        children: propTypes.exports.func,
+        accept: propTypes.exports.oneOfType([propTypes.exports.string, propTypes.exports.arrayOf(propTypes.exports.string)]),
+        multiple: propTypes.exports.bool,
+        preventDropOnDocument: propTypes.exports.bool,
+        noClick: propTypes.exports.bool,
+        noKeyboard: propTypes.exports.bool,
+        noDrag: propTypes.exports.bool,
+        noDragEventsBubbling: propTypes.exports.bool,
+        minSize: propTypes.exports.number,
+        maxSize: propTypes.exports.number,
+        disabled: propTypes.exports.bool,
+        getFilesFromEvent: propTypes.exports.func,
+        onFileDialogCancel: propTypes.exports.func,
+        onDragEnter: propTypes.exports.func,
+        onDragLeave: propTypes.exports.func,
+        onDragOver: propTypes.exports.func,
+        onDrop: propTypes.exports.func,
+        onDropAccepted: propTypes.exports.func,
+        onDropRejected: propTypes.exports.func
+    };
+    var initialState$2 = {
+        isFocused: false,
+        isFileDialogActive: false,
+        isDragActive: false,
+        isDragAccept: false,
+        isDragReject: false,
+        draggedFiles: [],
+        acceptedFiles: [],
+        fileRejections: []
+    };
+
+    function useDropzone() {
+        var _ref2 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
+            accept = _ref2.accept,
+            _ref2$disabled = _ref2.disabled,
+            disabled2 = _ref2$disabled === void 0 ? false : _ref2$disabled,
+            _ref2$getFilesFromEve = _ref2.getFilesFromEvent,
+            getFilesFromEvent = _ref2$getFilesFromEve === void 0 ? fromEvent : _ref2$getFilesFromEve,
+            _ref2$maxSize = _ref2.maxSize,
+            maxSize = _ref2$maxSize === void 0 ? Infinity : _ref2$maxSize,
+            _ref2$minSize = _ref2.minSize,
+            minSize = _ref2$minSize === void 0 ? 0 : _ref2$minSize,
+            _ref2$multiple = _ref2.multiple,
+            multiple = _ref2$multiple === void 0 ? true : _ref2$multiple,
+            onDragEnter = _ref2.onDragEnter,
+            onDragLeave = _ref2.onDragLeave,
+            onDragOver = _ref2.onDragOver,
+            onDrop = _ref2.onDrop,
+            onDropAccepted = _ref2.onDropAccepted,
+            onDropRejected = _ref2.onDropRejected,
+            onFileDialogCancel = _ref2.onFileDialogCancel,
+            _ref2$preventDropOnDo = _ref2.preventDropOnDocument,
+            preventDropOnDocument = _ref2$preventDropOnDo === void 0 ? true : _ref2$preventDropOnDo,
+            _ref2$noClick = _ref2.noClick,
+            noClick = _ref2$noClick === void 0 ? false : _ref2$noClick,
+            _ref2$noKeyboard = _ref2.noKeyboard,
+            noKeyboard = _ref2$noKeyboard === void 0 ? false : _ref2$noKeyboard,
+            _ref2$noDrag = _ref2.noDrag,
+            noDrag = _ref2$noDrag === void 0 ? false : _ref2$noDrag,
+            _ref2$noDragEventsBub = _ref2.noDragEventsBubbling,
+            noDragEventsBubbling = _ref2$noDragEventsBub === void 0 ? false : _ref2$noDragEventsBub;
+        var rootRef = React.useRef(null);
+        var inputRef = React.useRef(null);
+        var _useReducer = React.useReducer(reducer, initialState$2),
+            _useReducer2 = _slicedToArray$8(_useReducer, 2),
+            state = _useReducer2[0],
+            dispatch2 = _useReducer2[1];
+        var isFocused = state.isFocused,
+            isFileDialogActive = state.isFileDialogActive,
+            draggedFiles = state.draggedFiles;
+        var openFileDialog = React.useCallback(function() {
+            if (inputRef.current) {
+                dispatch2({
+                    type: "openDialog"
+                });
+                inputRef.current.value = null;
+                inputRef.current.click();
             }
-            const x2 = roundByDPR(elements.floating, data2.x);
-            const y2 = roundByDPR(elements.floating, data2.y);
-            if (transform) {
-                return {
-                    ...initialStyles,
-                    transform: "translate(" + x2 + "px, " + y2 + "px)",
-                    ...getDPR(elements.floating) >= 1.5 && {
-                        willChange: "transform"
+        }, [dispatch2]);
+        var onWindowFocus = function onWindowFocus2() {
+            if (isFileDialogActive) {
+                setTimeout(function() {
+                    if (inputRef.current) {
+                        var files = inputRef.current.files;
+                        if (!files.length) {
+                            dispatch2({
+                                type: "closeDialog"
+                            });
+                            if (typeof onFileDialogCancel === "function") {
+                                onFileDialogCancel();
+                            }
+                        }
                     }
-                };
+                }, 300);
             }
-            return {
-                position: strategy,
-                left: x2,
-                top: y2
+        };
+        React.useEffect(function() {
+            window.addEventListener("focus", onWindowFocus, false);
+            return function() {
+                window.removeEventListener("focus", onWindowFocus, false);
             };
-        }, [strategy, transform, elements.floating, data2.x, data2.y]);
-        return React__namespace.useMemo(() => ({
-            ...data2,
-            update: update2,
-            refs,
-            elements,
-            floatingStyles
-        }), [data2, update2, refs, elements, floatingStyles]);
-    }
-    const SafeReact = {
-        ...React__namespace
-    };
-    const useInsertionEffect = SafeReact.useInsertionEffect;
-    const useSafeInsertionEffect = useInsertionEffect || ((fn2) => fn2());
-
-    function useEffectEvent(callback) {
-        const ref2 = React__namespace.useRef(() => {});
-        useSafeInsertionEffect(() => {
-            ref2.current = callback;
-        });
-        return React__namespace.useCallback(function() {
-            for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {
-                args[_key] = arguments[_key];
+        }, [inputRef, isFileDialogActive, onFileDialogCancel]);
+        var onKeyDownCb = React.useCallback(function(event2) {
+            if (!rootRef.current || !rootRef.current.isEqualNode(event2.target)) {
+                return;
             }
-            return ref2.current == null ? void 0 : ref2.current(...args);
-        }, []);
-    }
-    var index$2 = typeof document !== "undefined" ? React.useLayoutEffect : React.useEffect;
-    let serverHandoffComplete = false;
-    let count$1 = 0;
-    const genId = () => "floating-ui-" + Math.random().toString(36).slice(2, 6) + count$1++;
-
-    function useFloatingId() {
-        const [id2, setId] = React__namespace.useState(() => serverHandoffComplete ? genId() : void 0);
-        index$2(() => {
-            if (id2 == null) {
-                setId(genId());
+            if (event2.keyCode === 32 || event2.keyCode === 13) {
+                event2.preventDefault();
+                openFileDialog();
             }
+        }, [rootRef, inputRef]);
+        var onFocusCb = React.useCallback(function() {
+            dispatch2({
+                type: "focus"
+            });
         }, []);
-        React__namespace.useEffect(() => {
-            serverHandoffComplete = true;
+        var onBlurCb = React.useCallback(function() {
+            dispatch2({
+                type: "blur"
+            });
         }, []);
-        return id2;
-    }
-    const useReactId = SafeReact.useId;
-    const useId = useReactId || useFloatingId;
-
-    function createPubSub() {
-        const map2 = /* @__PURE__ */ new Map();
-        return {
-            emit(event2, data2) {
-                var _map$get;
-                (_map$get = map2.get(event2)) == null || _map$get.forEach((handler) => handler(data2));
-            },
-            on(event2, listener2) {
-                map2.set(event2, [...map2.get(event2) || [], listener2]);
-            },
-            off(event2, listener2) {
-                var _map$get2;
-                map2.set(event2, ((_map$get2 = map2.get(event2)) == null ? void 0 : _map$get2.filter((l2) => l2 !== listener2)) || []);
+        var onClickCb = React.useCallback(function() {
+            if (noClick) {
+                return;
+            }
+            if (isIeOrEdge()) {
+                setTimeout(openFileDialog, 0);
+            } else {
+                openFileDialog();
+            }
+        }, [inputRef, noClick]);
+        var dragTargetsRef = React.useRef([]);
+        var onDocumentDrop = function onDocumentDrop2(event2) {
+            if (rootRef.current && rootRef.current.contains(event2.target)) {
+                return;
             }
+            event2.preventDefault();
+            dragTargetsRef.current = [];
         };
-    }
-    const FloatingNodeContext = /* @__PURE__ */ React__namespace.createContext(null);
-    const FloatingTreeContext = /* @__PURE__ */ React__namespace.createContext(null);
-    const useFloatingParentNodeId = () => {
-        var _React$useContext;
-        return ((_React$useContext = React__namespace.useContext(FloatingNodeContext)) == null ? void 0 : _React$useContext.id) || null;
-    };
-    const useFloatingTree = () => React__namespace.useContext(FloatingTreeContext);
-
-    function useFloating(options) {
-        var _options$elements;
-        if (options === void 0) {
-            options = {};
-        }
-        const {
-            open = false,
-                onOpenChange: unstable_onOpenChange,
-                nodeId
-        } = options;
-        const [_domReference, setDomReference] = React__namespace.useState(null);
-        const [positionReference, _setPositionReference] = React__namespace.useState(null);
-        const optionDomReference = (_options$elements = options.elements) == null ? void 0 : _options$elements.reference;
-        const domReference = optionDomReference || _domReference;
-        index$2(() => {
-            if (domReference) {
-                domReferenceRef.current = domReference;
+        React.useEffect(function() {
+            if (preventDropOnDocument) {
+                document.addEventListener("dragover", onDocumentDragOver, false);
+                document.addEventListener("drop", onDocumentDrop, false);
             }
-        }, [domReference]);
-        const position2 = useFloating$1({
-            ...options,
-            elements: {
-                ...options.elements,
-                ...positionReference && {
-                    reference: positionReference
+            return function() {
+                if (preventDropOnDocument) {
+                    document.removeEventListener("dragover", onDocumentDragOver);
+                    document.removeEventListener("drop", onDocumentDrop);
                 }
+            };
+        }, [rootRef, preventDropOnDocument]);
+        var onDragEnterCb = React.useCallback(function(event2) {
+            event2.preventDefault();
+            event2.persist();
+            stopPropagation(event2);
+            dragTargetsRef.current = [].concat(_toConsumableArray$2(dragTargetsRef.current), [event2.target]);
+            if (isEvtWithFiles(event2)) {
+                Promise.resolve(getFilesFromEvent(event2)).then(function(draggedFiles2) {
+                    if (isPropagationStopped(event2) && !noDragEventsBubbling) {
+                        return;
+                    }
+                    dispatch2({
+                        draggedFiles: draggedFiles2,
+                        isDragActive: true,
+                        type: "setDraggedFiles"
+                    });
+                    if (onDragEnter) {
+                        onDragEnter(event2);
+                    }
+                });
             }
-        });
-        const tree = useFloatingTree();
-        const nested = useFloatingParentNodeId() != null;
-        const onOpenChange = useEffectEvent((open2, event2, reason) => {
-            dataRef.current.openEvent = open2 ? event2 : void 0;
-            events2.emit("openchange", {
-                open: open2,
-                event: event2,
-                reason,
-                nested
+        }, [getFilesFromEvent, onDragEnter, noDragEventsBubbling]);
+        var onDragOverCb = React.useCallback(function(event2) {
+            event2.preventDefault();
+            event2.persist();
+            stopPropagation(event2);
+            if (event2.dataTransfer) {
+                try {
+                    event2.dataTransfer.dropEffect = "copy";
+                } catch (_unused) {}
+            }
+            if (isEvtWithFiles(event2) && onDragOver) {
+                onDragOver(event2);
+            }
+            return false;
+        }, [onDragOver, noDragEventsBubbling]);
+        var onDragLeaveCb = React.useCallback(function(event2) {
+            event2.preventDefault();
+            event2.persist();
+            stopPropagation(event2);
+            var targets = dragTargetsRef.current.filter(function(target) {
+                return rootRef.current && rootRef.current.contains(target);
             });
-            unstable_onOpenChange == null || unstable_onOpenChange(open2, event2, reason);
-        });
-        const domReferenceRef = React__namespace.useRef(null);
-        const dataRef = React__namespace.useRef({});
-        const events2 = React__namespace.useState(() => createPubSub())[0];
-        const floatingId = useId();
-        const setPositionReference = React__namespace.useCallback((node2) => {
-            const computedPositionReference = isElement$1(node2) ? {
-                getBoundingClientRect: () => node2.getBoundingClientRect(),
-                contextElement: node2
-            } : node2;
-            _setPositionReference(computedPositionReference);
-            position2.refs.setReference(computedPositionReference);
-        }, [position2.refs]);
-        const setReference = React__namespace.useCallback((node2) => {
-            if (isElement$1(node2) || node2 === null) {
-                domReferenceRef.current = node2;
-                setDomReference(node2);
+            var targetIdx = targets.indexOf(event2.target);
+            if (targetIdx !== -1) {
+                targets.splice(targetIdx, 1);
             }
-            if (isElement$1(position2.refs.reference.current) || position2.refs.reference.current === null || node2 !== null && !isElement$1(node2)) {
-                position2.refs.setReference(node2);
+            dragTargetsRef.current = targets;
+            if (targets.length > 0) {
+                return;
             }
-        }, [position2.refs]);
-        const refs = React__namespace.useMemo(() => ({
-            ...position2.refs,
-            setReference,
-            setPositionReference,
-            domReference: domReferenceRef
-        }), [position2.refs, setReference, setPositionReference]);
-        const elements = React__namespace.useMemo(() => ({
-            ...position2.elements,
-            domReference
-        }), [position2.elements, domReference]);
-        const context2 = React__namespace.useMemo(() => ({
-            ...position2,
-            refs,
-            elements,
-            dataRef,
-            nodeId,
-            floatingId,
-            events: events2,
-            open,
-            onOpenChange
-        }), [position2, nodeId, floatingId, events2, open, onOpenChange, refs, elements]);
-        index$2(() => {
-            const node2 = tree == null ? void 0 : tree.nodesRef.current.find((node3) => node3.id === nodeId);
-            if (node2) {
-                node2.context = context2;
+            dispatch2({
+                isDragActive: false,
+                type: "setDraggedFiles",
+                draggedFiles: []
+            });
+            if (isEvtWithFiles(event2) && onDragLeave) {
+                onDragLeave(event2);
             }
-        });
-        return React__namespace.useMemo(() => ({
-            ...position2,
-            context: context2,
-            refs,
-            elements
-        }), [position2, refs, elements, context2]);
-    }
-    const ACTIVE_KEY = "active";
-    const SELECTED_KEY = "selected";
-
-    function mergeProps(userProps, propsList, elementKey) {
-        const map2 = /* @__PURE__ */ new Map();
-        const isItem2 = elementKey === "item";
-        let domUserProps = userProps;
-        if (isItem2 && userProps) {
-            const {
-                [ACTIVE_KEY]: _2,
-                [SELECTED_KEY]: __,
-                ...validProps
-            } = userProps;
-            domUserProps = validProps;
-        }
-        return {
-            ...elementKey === "floating" && {
-                tabIndex: -1
-            },
-            ...domUserProps,
-            ...propsList.map((value) => {
-                const propsOrGetProps = value ? value[elementKey] : null;
-                if (typeof propsOrGetProps === "function") {
-                    return userProps ? propsOrGetProps(userProps) : null;
-                }
-                return propsOrGetProps;
-            }).concat(userProps).reduce((acc, props) => {
-                if (!props) {
-                    return acc;
-                }
-                Object.entries(props).forEach((_ref2) => {
-                    let [key, value] = _ref2;
-                    if (isItem2 && [ACTIVE_KEY, SELECTED_KEY].includes(key)) {
+        }, [rootRef, onDragLeave, noDragEventsBubbling]);
+        var onDropCb = React.useCallback(function(event2) {
+            event2.preventDefault();
+            event2.persist();
+            stopPropagation(event2);
+            dragTargetsRef.current = [];
+            if (isEvtWithFiles(event2)) {
+                Promise.resolve(getFilesFromEvent(event2)).then(function(files) {
+                    if (isPropagationStopped(event2) && !noDragEventsBubbling) {
                         return;
                     }
-                    if (key.indexOf("on") === 0) {
-                        if (!map2.has(key)) {
-                            map2.set(key, []);
-                        }
-                        if (typeof value === "function") {
-                            var _map$get;
-                            (_map$get = map2.get(key)) == null || _map$get.push(value);
-                            acc[key] = function() {
-                                var _map$get2;
-                                for (var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++) {
-                                    args[_key] = arguments[_key];
-                                }
-                                return (_map$get2 = map2.get(key)) == null ? void 0 : _map$get2.map((fn2) => fn2(...args)).find((val) => val !== void 0);
-                            };
+                    var acceptedFiles = [];
+                    var fileRejections = [];
+                    files.forEach(function(file) {
+                        var _fileAccepted = fileAccepted(file, accept),
+                            _fileAccepted2 = _slicedToArray$8(_fileAccepted, 2),
+                            accepted = _fileAccepted2[0],
+                            acceptError = _fileAccepted2[1];
+                        var _fileMatchSize = fileMatchSize(file, minSize, maxSize),
+                            _fileMatchSize2 = _slicedToArray$8(_fileMatchSize, 2),
+                            sizeMatch = _fileMatchSize2[0],
+                            sizeError = _fileMatchSize2[1];
+                        if (accepted && sizeMatch) {
+                            acceptedFiles.push(file);
+                        } else {
+                            var errors = [acceptError, sizeError].filter(function(e3) {
+                                return e3;
+                            });
+                            fileRejections.push({
+                                file,
+                                errors
+                            });
                         }
-                    } else {
-                        acc[key] = value;
+                    });
+                    if (!multiple && acceptedFiles.length > 1) {
+                        acceptedFiles.forEach(function(file) {
+                            fileRejections.push({
+                                file,
+                                errors: [TOO_MANY_FILES_REJECTION]
+                            });
+                        });
+                        acceptedFiles.splice(0);
+                    }
+                    dispatch2({
+                        acceptedFiles,
+                        fileRejections,
+                        type: "setFiles"
+                    });
+                    if (onDrop) {
+                        onDrop(acceptedFiles, fileRejections, event2);
+                    }
+                    if (fileRejections.length > 0 && onDropRejected) {
+                        onDropRejected(fileRejections, event2);
+                    }
+                    if (acceptedFiles.length > 0 && onDropAccepted) {
+                        onDropAccepted(acceptedFiles, event2);
                     }
                 });
-                return acc;
-            }, {})
+            }
+            dispatch2({
+                type: "reset"
+            });
+        }, [multiple, accept, minSize, maxSize, getFilesFromEvent, onDrop, onDropAccepted, onDropRejected, noDragEventsBubbling]);
+        var composeHandler = function composeHandler2(fn2) {
+            return disabled2 ? null : fn2;
+        };
+        var composeKeyboardHandler = function composeKeyboardHandler2(fn2) {
+            return noKeyboard ? null : composeHandler(fn2);
         };
+        var composeDragHandler = function composeDragHandler2(fn2) {
+            return noDrag ? null : composeHandler(fn2);
+        };
+        var stopPropagation = function stopPropagation2(event2) {
+            if (noDragEventsBubbling) {
+                event2.stopPropagation();
+            }
+        };
+        var getRootProps = React.useMemo(function() {
+            return function() {
+                var _ref3 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
+                    _ref3$refKey = _ref3.refKey,
+                    refKey = _ref3$refKey === void 0 ? "ref" : _ref3$refKey,
+                    onKeyDown = _ref3.onKeyDown,
+                    onFocus = _ref3.onFocus,
+                    onBlur = _ref3.onBlur,
+                    onClick = _ref3.onClick,
+                    onDragEnter2 = _ref3.onDragEnter,
+                    onDragOver2 = _ref3.onDragOver,
+                    onDragLeave2 = _ref3.onDragLeave,
+                    onDrop2 = _ref3.onDrop,
+                    rest = _objectWithoutProperties$1(_ref3, ["refKey", "onKeyDown", "onFocus", "onBlur", "onClick", "onDragEnter", "onDragOver", "onDragLeave", "onDrop"]);
+                return _objectSpread$5(_defineProperty$n({
+                    onKeyDown: composeKeyboardHandler(composeEventHandlers(onKeyDown, onKeyDownCb)),
+                    onFocus: composeKeyboardHandler(composeEventHandlers(onFocus, onFocusCb)),
+                    onBlur: composeKeyboardHandler(composeEventHandlers(onBlur, onBlurCb)),
+                    onClick: composeHandler(composeEventHandlers(onClick, onClickCb)),
+                    onDragEnter: composeDragHandler(composeEventHandlers(onDragEnter2, onDragEnterCb)),
+                    onDragOver: composeDragHandler(composeEventHandlers(onDragOver2, onDragOverCb)),
+                    onDragLeave: composeDragHandler(composeEventHandlers(onDragLeave2, onDragLeaveCb)),
+                    onDrop: composeDragHandler(composeEventHandlers(onDrop2, onDropCb))
+                }, refKey, rootRef), !disabled2 && !noKeyboard ? {
+                    tabIndex: 0
+                } : {}, {}, rest);
+            };
+        }, [rootRef, onKeyDownCb, onFocusCb, onBlurCb, onClickCb, onDragEnterCb, onDragOverCb, onDragLeaveCb, onDropCb, noKeyboard, noDrag, disabled2]);
+        var onInputElementClick = React.useCallback(function(event2) {
+            event2.stopPropagation();
+        }, []);
+        var getInputProps = React.useMemo(function() {
+            return function() {
+                var _ref4 = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
+                    _ref4$refKey = _ref4.refKey,
+                    refKey = _ref4$refKey === void 0 ? "ref" : _ref4$refKey,
+                    onChange2 = _ref4.onChange,
+                    onClick = _ref4.onClick,
+                    rest = _objectWithoutProperties$1(_ref4, ["refKey", "onChange", "onClick"]);
+                var inputProps = _defineProperty$n({
+                    accept,
+                    multiple,
+                    type: "file",
+                    style: {
+                        display: "none"
+                    },
+                    onChange: composeHandler(composeEventHandlers(onChange2, onDropCb)),
+                    onClick: composeHandler(composeEventHandlers(onClick, onInputElementClick)),
+                    autoComplete: "off",
+                    tabIndex: -1
+                }, refKey, inputRef);
+                return _objectSpread$5({}, inputProps, {}, rest);
+            };
+        }, [inputRef, accept, multiple, onDropCb, disabled2]);
+        var fileCount = draggedFiles.length;
+        var isDragAccept = fileCount > 0 && allFilesAccepted({
+            files: draggedFiles,
+            accept,
+            minSize,
+            maxSize,
+            multiple
+        });
+        var isDragReject = fileCount > 0 && !isDragAccept;
+        return _objectSpread$5({}, state, {
+            isDragAccept,
+            isDragReject,
+            isFocused: isFocused && !disabled2,
+            getRootProps,
+            getInputProps,
+            rootRef,
+            inputRef,
+            open: composeHandler(openFileDialog)
+        });
     }
 
-    function useInteractions(propsList) {
-        if (propsList === void 0) {
-            propsList = [];
+    function reducer(state, action) {
+        switch (action.type) {
+            case "focus":
+                return _objectSpread$5({}, state, {
+                    isFocused: true
+                });
+            case "blur":
+                return _objectSpread$5({}, state, {
+                    isFocused: false
+                });
+            case "openDialog":
+                return _objectSpread$5({}, state, {
+                    isFileDialogActive: true
+                });
+            case "closeDialog":
+                return _objectSpread$5({}, state, {
+                    isFileDialogActive: false
+                });
+            case "setDraggedFiles":
+                var isDragActive = action.isDragActive,
+                    draggedFiles = action.draggedFiles;
+                return _objectSpread$5({}, state, {
+                    draggedFiles,
+                    isDragActive
+                });
+            case "setFiles":
+                return _objectSpread$5({}, state, {
+                    acceptedFiles: action.acceptedFiles,
+                    fileRejections: action.fileRejections
+                });
+            case "reset":
+                return _objectSpread$5({}, state, {
+                    isFileDialogActive: false,
+                    isDragActive: false,
+                    draggedFiles: [],
+                    acceptedFiles: [],
+                    fileRejections: []
+                });
+            default:
+                return state;
         }
-        const deps = propsList;
-        const getReferenceProps = React__namespace.useCallback(
-            (userProps) => mergeProps(userProps, propsList, "reference"),
-            deps
-        );
-        const getFloatingProps = React__namespace.useCallback(
-            (userProps) => mergeProps(userProps, propsList, "floating"),
-            deps
-        );
-        const getItemProps = React__namespace.useCallback(
-            (userProps) => mergeProps(userProps, propsList, "item"),
-            propsList.map((key) => key == null ? void 0 : key.item)
-        );
-        return React__namespace.useMemo(() => ({
-            getReferenceProps,
-            getFloatingProps,
-            getItemProps
-        }), [getReferenceProps, getFloatingProps, getItemProps]);
     }
-    const componentRoleToAriaRoleMap = /* @__PURE__ */ new Map([
-        ["select", "listbox"],
-        ["combobox", "listbox"],
-        ["label", false]
-    ]);
+    const DROPZONE_ALLOWED_MIME_TYPES = ".csv, text/csv, application/vnd.openxmlformats-officedocument.spreadsheetml.sheet, application/vnd.ms-excel, application/csv, text/x-csv, application/x-csv, text/comma-separated-values, text/x-comma-separated-values";
+    const Dropzone = styled__default.default.div`
+    display: flex;
+    flex: 1 1 auto;
+    align-items: center;
+    justify-content: center;
 
-    function useRole(context2, props) {
-        var _componentRoleToAriaR;
-        if (props === void 0) {
-            props = {};
-        }
-        const {
-            open,
-            floatingId
-        } = context2;
+    margin-top: 20px;
+
+    color: ${(props) => props.theme.colors.text};
+
+    border: 1px dashed ${(props) => props.isDragActive ? props.theme.colors.primary : props.theme.colors.grey3};
+    border-radius: 0.25rem;
+
+    :hover {
+        background-color: ${(props) => props.theme.colors.grey1};
+    }
+
+    :active,
+    :focus {
+        background-color: ${(props) => props.theme.colors.grey2};
+    }
+`;
+    const DropzoneMessage = styled__default.default.span`
+    max-width: 400px;
+    padding: 1.5rem;
+
+    font-family: Manrope, sans-serif;
+    font-weight: 300;
+    text-align: center;
+`;
+
+    function UploadDropzone$1(props) {
+        var _a3;
+        React.useEffect(() => {
+            if (!props.enablePaste) {
+                return;
+            }
+            const handlePaste = (ev) => {
+                const blob = new Blob([ev.clipboardData.getData("Text")], {
+                    type: "text/plain"
+                });
+                const file = new File([blob], "pasted_data", {
+                    type: "text/plain"
+                });
+                props.onDrop([file]);
+            };
+            document.addEventListener("paste", handlePaste);
+            return () => document.removeEventListener("paste", handlePaste);
+        }, [props]);
         const {
-            enabled = true,
-                role = "dialog"
-        } = props;
-        const ariaRole = (_componentRoleToAriaR = componentRoleToAriaRoleMap.get(role)) != null ? _componentRoleToAriaR : role;
-        const referenceId = useId();
-        const parentId = useFloatingParentNodeId();
-        const isNested = parentId != null;
-        return React__namespace.useMemo(() => {
-            if (!enabled)
-                return {};
-            const floatingProps = {
-                id: floatingId,
-                ...ariaRole && {
-                    role: ariaRole
+            getRootProps,
+            getInputProps,
+            isDragActive
+        } = useDropzone({
+            accept: (_a3 = props.accept) !== null && _a3 !== void 0 ? _a3 : DROPZONE_ALLOWED_MIME_TYPES,
+            multiple: false,
+            onDrop: props.onDrop
+        });
+        return jsxRuntime.exports.jsxs(Dropzone, Object.assign({}, getRootProps(), {
+            className: props.className,
+            isDragActive,
+            style: props.style,
+            children: [jsxRuntime.exports.jsx("input", Object.assign({}, getInputProps())), jsxRuntime.exports.jsxs(DropzoneMessage, {
+                children: ["Drop your file, ", jsxRuntime.exports.jsx("br", {}), "paste it ", jsxRuntime.exports.jsx("br", {}), "or click here to upload"]
+            })]
+        }));
+    }
+    styled__default.default.div`
+    display: flex;
+    flex-direction: column;
+
+    width: 100%;
+    padding: 1rem;
+
+    color: ${(props) => props.theme.colors.error};
+
+    background-color: ${(props) => props.theme.colors.background};
+`;
+    styled__default.default.div`
+    overflow: scroll;
+    display: flex;
+    flex-direction: column;
+
+    width: 100%;
+    max-height: 125px;
+    margin: 2rem 0;
+    padding: 0.5rem;
+
+    color: ${(props) => props.theme.colors.background};
+
+    background-color: ${(props) => props.theme.colors.errorHover};
+`;
+    styled__default.default.p`
+    color: ${(props) => props.theme.colors.error};
+`;
+    const NodeContent = styled__default.default.li`
+    margin-left: 0.35rem;
+    border-left: thin solid ${(props) => props.theme.colors.grey6};
+
+    &::before {
+        content: '';
+
+        display: inline-block;
+
+        width: 0.9rem;
+        height: 0.8rem;
+        margin-right: 0.1rem;
+
+        vertical-align: top;
+
+        border-bottom: thin solid ${(props) => props.theme.colors.grey6};
+    }
+
+    &:last-child {
+        border-left: none;
+
+        &::before {
+            border-left: thin solid ${(props) => props.theme.colors.grey6};
+        }
+    }
+`;
+    const Cell$1 = styled__default.default.span`
+    cursor: ${(props) => props.selectionAllowed ? "pointer" : "normal"};
+    font-weight: ${(props) => props.isLeaf ? 300 : 400};
+    color: ${(props) => {
+    if (props.selected) {
+      return props.theme.colors.primary;
+    }
+    return props.isLeaf ? props.theme.colors.grey6 : props.theme.colors.grey5;
+  }};
+`;
+    const CircleIcon = styled__default.default(Circle$1)`
+    width: 0.5rem;
+    height: 0.5rem;
+    margin-right: 0.4rem;
+
+    color: ${(props) => props.selected ? props.theme.colors.primary : props.theme.colors.grey6};
+    vertical-align: middle;
+`;
+    const grow = styled.keyframes`
+    0% {
+        transform: scaleY(0);
+        opacity: 0;
+    }
+    100% {
+        transform: scaleY(1);
+        opacity: 1;
+    }
+`;
+    const contract = styled.keyframes`
+    100% {
+        transform: scaleY(1);
+        opacity: 1;
+    }
+    0% {
+        transform: scaleY(0);
+        opacity: 0;
+    }
+`;
+    const NodeWrapper = styled__default.default.ul`
+    transform-origin: top center;
+
+    display: ${(props) => props.open ? "block" : "none"};
+
+    margin: 0;
+    margin-left: 1rem;
+    padding: 0;
+    padding-bottom: 1rem;
+
+    list-style: none;
+
+    animation: ${(props) => props.open ? grow : contract} 300ms
+        ${(props) => props.open ? "ease-out forwards" : "ease-in forwards"};
+`;
+
+    function Branch(props) {
+        const theme2 = useClTheme();
+        const [open, setOpen] = React.useState(props.open || false);
+        const toggle = () => {
+            if (props.content) {
+                setOpen(!open);
+            }
+        };
+        const select = () => {
+            props.selectNode(props.content.id);
+        };
+        const selectionAllowed = props.allowSelectCategory && props.content.children && props.content.children.length > 0 || props.allowSelectLeaf && (!props.content.children || props.content.children.length === 0);
+        return jsxRuntime.exports.jsxs(NodeContent, {
+            className: props.className,
+            style: props.style,
+            children: [jsxRuntime.exports.jsx(CircleIcon, {
+                selected: props.content.id === props.selectedNodeId
+            }), jsxRuntime.exports.jsx(Cell$1, {
+                isLeaf: !props.content.children || props.content.children.length === 0,
+                onClick: selectionAllowed ? select : toggle,
+                selected: props.content.id === props.selectedNodeId,
+                selectionAllowed,
+                children: props.content.label
+            }), props.content.children && props.content.children.length > 0 && jsxRuntime.exports.jsx(Chevron$2, {
+                isOpen: open,
+                onClick: toggle,
+                style: {
+                    color: theme2.colors.grey5,
+                    cursor: "pointer",
+                    height: "0.8rem",
+                    marginLeft: "0.5rem",
+                    verticalAlign: "middle",
+                    width: "0.8rem"
                 }
-            };
-            if (ariaRole === "tooltip" || role === "label") {
-                return {
-                    reference: {
-                        ["aria-" + (role === "label" ? "labelledby" : "describedby")]: open ? floatingId : void 0
-                    },
-                    floating: floatingProps
-                };
+            }), jsxRuntime.exports.jsx(NodeWrapper, {
+                open,
+                children: props.content.children && props.content.children.length > 0 && props.content.children.map((nodeObj) => jsxRuntime.exports.jsx(Branch, {
+                    allowSelectCategory: props.allowSelectCategory,
+                    allowSelectLeaf: props.allowSelectLeaf,
+                    content: nodeObj,
+                    selectCategory: props.selectCategory,
+                    selectNode: props.selectNode,
+                    selectedNodeId: props.selectedNodeId
+                }, nodeObj.id))
+            })]
+        });
+    }
+    const Wrapper$8 = styled__default.default.div`
+    overflow: scroll;
+`;
+    const Root = styled__default.default.div`
+    cursor: pointer;
+    margin-left: 1rem;
+`;
+
+    function HierarchySelector$1(props) {
+        const theme2 = useClTheme();
+        const [rootOpen, setRootOpen] = React.useState(props.rootOpen || false);
+        const [selectedNodeId, setSelectedNodeId] = React.useState(props.selected);
+        React.useEffect(() => {
+            if (props.selected) {
+                setSelectedNodeId(props.selected);
             }
-            return {
-                reference: {
-                    "aria-expanded": open ? "true" : "false",
-                    "aria-haspopup": ariaRole === "alertdialog" ? "dialog" : ariaRole,
-                    "aria-controls": open ? floatingId : void 0,
-                    ...ariaRole === "listbox" && {
-                        role: "combobox"
-                    },
-                    ...ariaRole === "menu" && {
-                        id: referenceId
-                    },
-                    ...ariaRole === "menu" && isNested && {
-                        role: "menuitem"
-                    },
-                    ...role === "select" && {
-                        "aria-autocomplete": "none"
-                    },
-                    ...role === "combobox" && {
-                        "aria-autocomplete": "list"
-                    }
-                },
-                floating: {
-                    ...floatingProps,
-                    ...ariaRole === "menu" && {
-                        "aria-labelledby": referenceId
+        }, [props.selected]);
+        const toggle = () => {
+            setRootOpen(!rootOpen);
+        };
+        const selectNode = (nodeId) => {
+            var _a3;
+            setSelectedNodeId(nodeId);
+            (_a3 = props.onSelect) === null || _a3 === void 0 ? void 0 : _a3.call(props, nodeId);
+        };
+        const {
+            label,
+            id: id2,
+            children: children2
+        } = props.rootNode;
+        return jsxRuntime.exports.jsxs(Wrapper$8, {
+            className: props.className,
+            style: props.style,
+            children: [jsxRuntime.exports.jsxs(Root, {
+                children: [jsxRuntime.exports.jsx(CircleIcon, {
+                    selected: id2 === selectedNodeId
+                }), jsxRuntime.exports.jsx(Cell$1, {
+                    onClick: props.allowSelectCategory || children2.length === 0 ? () => selectNode(id2) : toggle,
+                    selected: id2 === selectedNodeId,
+                    children: label
+                }), children2.length > 0 && jsxRuntime.exports.jsx(Chevron$2, {
+                    isOpen: rootOpen,
+                    onClick: toggle,
+                    style: {
+                        color: theme2.colors.grey5,
+                        cursor: "pointer",
+                        height: "0.8rem",
+                        marginLeft: "0.5rem",
+                        verticalAlign: "middle",
+                        width: "0.8rem"
                     }
-                },
-                item(_ref2) {
-                    let {
-                        active,
-                        selected
-                    } = _ref2;
-                    const commonProps = {
-                        role: "option",
-                        ...active && {
-                            id: floatingId + "-option"
-                        }
-                    };
-                    switch (role) {
-                        case "select":
-                            return {
-                                ...commonProps,
-                                "aria-selected": active && selected
-                            };
-                        case "combobox": {
-                            return {
-                                ...commonProps,
-                                ...active && {
-                                    "aria-selected": true
-                                }
-                            };
-                        }
+                })]
+            }), jsxRuntime.exports.jsx(NodeWrapper, {
+                open: rootOpen,
+                children: children2 && children2.map((nodeObj) => jsxRuntime.exports.jsx(Branch, {
+                    allowSelectCategory: props.allowSelectCategory,
+                    allowSelectLeaf: props.allowSelectLeaf,
+                    content: nodeObj,
+                    open: rootOpen,
+                    selectNode,
+                    selectedNodeId
+                }, nodeObj.id))
+            })]
+        });
+    }
+    const Background$1 = styled__default.default.div`
+    position: fixed;
+    z-index: 2000;
+    top: 0;
+    left: 0;
+
+    display: flex;
+    align-items: center;
+    justify-content: center;
+
+    width: 100%;
+    height: 100%;
+
+    opacity: ${(props) => props.render ? 1 : 0};
+    background-color: ${(props) => props.theme.colors.modalBg};
+
+    transition: opacity ease-in 0.1s;
+`;
+    const ModalWrapper = styled__default.default.div`
+    overflow: hidden;
+    display: inline-flex;
+    flex-direction: column;
+
+    min-width: 20rem;
+    max-width: 80vw;
+    min-height: 10rem;
+    max-height: 80vh;
+    margin-top: ${(props) => props.render ? 0 : "-50px"};
+    padding: 1.75rem;
+
+    font-size: ${(props) => props.theme.font.size};
+
+    background-color: ${(props) => props.theme.colors.grey1};
+    border-radius: 0.25rem;
+    box-shadow: ${(props) => props.theme.shadow.medium};
+
+    transition: margin-top ease-in 0.1s;
+`;
+    styled__default.default.div`
+    display: flex;
+    flex: 0 0 auto;
+    justify-content: space-between;
+    margin-top: 1rem;
+`;
+    styled__default.default.div`
+    display: flex;
+    flex: 0 0 auto;
+    flex-direction: ${(props) => props.flexDirection || "column"};
+    justify-content: space-between;
+
+    margin-bottom: 1rem;
+`;
+
+    function Modal$1(props) {
+        var _a3;
+        const [mounted, setMounted] = React.useState(false);
+        const [renderModal, setRenderModal] = React.useState(false);
+        React.useEffect(() => {
+            setRenderModal(props.render);
+        }, [props.render]);
+        React.useEffect(() => {
+            if (renderModal) {
+                const keyHandler = (e3) => {
+                    if (e3.key === Key.ESCAPE && props.onAttemptClose) {
+                        props.onAttemptClose();
                     }
-                    return {};
-                }
-            };
-        }, [enabled, role, ariaRole, open, floatingId, referenceId, isNested]);
+                };
+                document.addEventListener("keydown", keyHandler);
+                return () => {
+                    document.removeEventListener("keydown", keyHandler);
+                };
+            }
+        }, [renderModal, props.onAttemptClose]);
+        if (!props.render && !mounted) {
+            return null;
+        }
+        const onTransitionEnd = () => {
+            setMounted(props.render);
+            if (!props.render && props.onClosed) {
+                props.onClosed();
+            }
+        };
+        const stopPropagation = (e3) => {
+            e3.stopPropagation();
+        };
+        return ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(Background$1, {
+            id: props.id,
+            onClick: props.onAttemptClose,
+            onTransitionEnd,
+            render: renderModal,
+            children: jsxRuntime.exports.jsx(ModalWrapper, {
+                className: `cl-modal-content ${(_a3 = props.className) !== null && _a3 !== void 0 ? _a3 : ""}`,
+                onClick: stopPropagation,
+                render: renderModal,
+                style: props.style,
+                children: props.children
+            })
+        }), document.body);
     }
     var __rest$9 = globalThis && globalThis.__rest || function(s2, e3) {
         var t2 = {};
         for (var p2 in s2)
             if (Object.prototype.hasOwnProperty.call(s2, p2) && e3.indexOf(p2) < 0)
                 t2[p2] = s2[p2];
         if (s2 != null && typeof Object.getOwnPropertySymbols === "function")
@@ -53482,31 +52499,20 @@
         });
         const {
             refs,
             floatingStyles,
             context: context2
         } = useFloating({
             open: isOpen,
-            middleware: [
-                flip(),
-                shift$1(),
-                size$1({
-                    apply({
-                        rects,
-                        elements
-                    }) {
-                        Object.assign(elements.floating.style, {
-                            width: `${rects.reference.width}px`
-                        });
-                    }
-                })
-            ],
+            middleware: [flip$2(), shift$1(), matchWidthToReference()],
             whileElementsMounted: isOpen ? autoUpdate : void 0
         });
-        const role = useRole(context2);
+        const role = useRole(context2, {
+            role: "listbox"
+        });
         const {
             getReferenceProps,
             getFloatingProps
         } = useInteractions([role]);
         const menuProps = getMenuProps();
         const setMenuRef = menuProps.ref;
         const setFloatingRef = refs.setFloating;
@@ -53521,19 +52527,18 @@
             maxRows,
             maxWidth,
             style: props.style,
             children: [jsxRuntime.exports.jsx(Tooltip$1, {
                 content: props.errorMsg,
                 disabled: !props.errorMsg,
                 styling: "error",
-                children: jsxRuntime.exports.jsxs(InputWrapper$3, Object.assign({
+                children: jsxRuntime.exports.jsxs(InputWrapper$3, {
                     isDisabled: props.disabled,
                     isOpen,
-                    ref: refs.setReference
-                }, getReferenceProps(), {
+                    ref: refs.setReference,
                     children: [jsxRuntime.exports.jsxs(TagWrapper, {
                         maxRows,
                         children: [selectedItems.map((selectedItem, index2) => jsxRuntime.exports.jsxs(Tag$1, Object.assign({
                             disabled: props.disabled
                         }, getSelectedItemProps({
                             index: index2,
                             selectedItem
@@ -53545,36 +52550,33 @@
                                 onClick: (e3) => {
                                     e3.stopPropagation();
                                     return removeSelectedItem(selectedItem);
                                 }
                             })]
                         }), selectedItem.value)), jsxRuntime.exports.jsx(Input$1, Object.assign({}, getInputProps(getDropdownProps({
                             preventKeyAction: isOpen
-                        })), {
+                        })), getReferenceProps(), {
                             disabled: props.disabled,
                             placeholder: props.placeholder,
                             size: props.size,
                             style: {
                                 flex: "1 1 5ch"
                             }
                         }))]
                     }), jsxRuntime.exports.jsx(ChevronButton, Object.assign({}, getToggleButtonProps(), {
                         children: jsxRuntime.exports.jsx(Chevron$2, {
                             disabled: props.disabled,
                             isOpen
                         })
                     }))]
-                }))
+                })
             }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsxs(DropdownList$1, Object.assign({}, menuProps, getFloatingProps(), {
                 ref: mergedRefs,
-                role: "listbox",
                 isOpen,
-                style: Object.assign(Object.assign(Object.assign({}, floatingStyles), floatingStyles.width && {
-                    width: parseFloat(floatingStyles.width)
-                }), {
+                style: Object.assign(Object.assign({}, floatingStyles), {
                     zIndex: 9999
                 }),
                 children: [filteredItems.length > 0 && filteredItems.map((item, index2) => React.createElement(ListItem, Object.assign({}, getItemProps({
                     index: index2,
                     item
                 }), {
                     hovered: index2 === highlightedIndex,
@@ -53691,25 +52693,18 @@
     margin-left: -1px;
     border-radius: 0 0 0.25rem 0.25rem;
     outline: 0;
     box-shadow: ${(props) => props.theme.shadow.light};
 `;
 
     function Select$1(props) {
-        var _a3, _b, _c, _d, _e2, _f;
-        const referenceElement = React.useRef(null);
-        const popperElement = React.useRef(null);
+        var _a3, _b, _c;
         const {
-            styles: styles2,
-            attributes: attributes2,
-            update: update2
-        } = usePopper$1(referenceElement.current, popperElement.current, {
-            modifiers: props.applySameWidthModifier === false ? [] : [sameWidthModifier],
-            placement: props.placement || "bottom-start"
-        });
+            applySameWidthModifier = true
+        } = props;
         const {
             isOpen,
             selectedItem,
             getToggleButtonProps,
             getMenuProps,
             highlightedIndex,
             getItemProps
@@ -53722,68 +52717,75 @@
                 var _a4;
                 const selected = changes.selectedItem;
                 (_a4 = props.onSelect) === null || _a4 === void 0 ? void 0 : _a4.call(props, selected);
             }
         }, "selectedItem" in props && {
             selectedItem: props.selectedItem
         }));
-        React.useEffect(() => {
-            if (isOpen && update2) {
-                update2();
-            }
-        }, [isOpen, update2]);
-        const buttonProps = getToggleButtonProps({
-            disabled: props.disabled
-        });
-        const setButtonRef = buttonProps.ref;
-        delete buttonProps.ref;
-        const setButtonReference = (value) => {
-            setButtonRef(value);
-            referenceElement.current = value;
-        };
+        const {
+            refs,
+            floatingStyles,
+            context: context2
+        } = useFloating({
+            open: isOpen,
+            placement: props.placement || "bottom-start",
+            middleware: [flip$2(), shift$1(), ...applySameWidthModifier ? [matchWidthToReference(2)] : []],
+            whileElementsMounted: isOpen ? autoUpdate : void 0
+        });
+        const role = useRole(context2, {
+            role: "listbox"
+        });
+        const {
+            getReferenceProps,
+            getFloatingProps
+        } = useInteractions([role]);
         const menuProps = getMenuProps();
         const setMenuRef = menuProps.ref;
-        delete menuProps.ref;
-        const setMenuReference = (value) => {
-            var _a4;
-            setMenuRef(value);
-            popperElement.current = value;
-            (_a4 = props.dropdownRef) === null || _a4 === void 0 ? void 0 : _a4.call(props, value);
-        };
+        const setFloatingRef = refs.setFloating;
+        const {
+            dropdownRef
+        } = props;
+        const mergedRefs = React__namespace.useCallback((node2) => {
+            setFloatingRef(node2);
+            setMenuRef(node2);
+            dropdownRef === null || dropdownRef === void 0 ? void 0 : dropdownRef(node2);
+        }, [setFloatingRef, setMenuRef, dropdownRef]);
         return jsxRuntime.exports.jsx(Tooltip$1, {
             content: props.errorMsg,
             disabled: !props.errorMsg,
             styling: "error",
             children: jsxRuntime.exports.jsxs(Wrapper$6, {
                 className: props.className,
                 isDisabled: props.disabled,
                 isErrored: !!props.errorMsg,
                 isOpen,
                 onClick: props.onClick,
                 style: props.style,
                 children: [jsxRuntime.exports.jsxs(SelectButton, Object.assign({
                     disabled: props.disabled,
                     isOpen
-                }, buttonProps, {
-                    ref: setButtonReference,
+                }, getToggleButtonProps({
+                    disabled: props.disabled
+                }), {
+                    ref: refs.setReference
+                }, getReferenceProps(), {
                     type: "button",
                     children: [jsxRuntime.exports.jsx(SelectedItem, {
                         size: props.size,
                         children: (_b = (_a3 = selectedItem === null ? props.placeholder : selectedItem === null || selectedItem === void 0 ? void 0 : selectedItem.label) !== null && _a3 !== void 0 ? _a3 : props.placeholder) !== null && _b !== void 0 ? _b : "Select"
                     }), jsxRuntime.exports.jsx(Chevron$2, {
                         disabled: props.disabled,
                         isOpen
                     })]
-                })), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(DropdownList, Object.assign({}, menuProps, attributes2.popper, {
-                    className: `${(_c = menuProps === null || menuProps === void 0 ? void 0 : menuProps.className) !== null && _c !== void 0 ? _c : ""} ${(_e2 = (_d = attributes2 === null || attributes2 === void 0 ? void 0 : attributes2.popper) === null || _d === void 0 ? void 0 : _d.className) !== null && _e2 !== void 0 ? _e2 : ""} ${props.itemClass}`,
+                })), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(DropdownList, Object.assign({}, menuProps, getFloatingProps(), {
+                    ref: mergedRefs,
+                    className: `${(_c = menuProps === null || menuProps === void 0 ? void 0 : menuProps.className) !== null && _c !== void 0 ? _c : ""} ${props.itemClass}`,
                     isOpen,
                     maxItems: props.maxItems,
-                    ref: setMenuReference,
-                    style: Object.assign(Object.assign({}, styles2.popper), {
-                        width: props.applySameWidthModifier === false ? void 0 : parseFloat((_f = styles2.popper) === null || _f === void 0 ? void 0 : _f.width) + 2,
+                    style: Object.assign(Object.assign({}, floatingStyles), {
                         zIndex: 9999
                     }),
                     children: props.items.map((item, index2) => {
                         const _a4 = getItemProps({
                                 index: index2,
                                 item
                             }),
@@ -54610,26 +53612,16 @@
                 return [...acc, sectionHeading, ...sectionItems];
             }
             return [...acc, item];
         }, []);
     }
 
     function SectionedList(props) {
-        var _a3, _b, _c, _d;
+        var _a3, _b, _c;
         const theme2 = useClTheme();
-        const referenceElement = React.useRef(null);
-        const popperElement = React.useRef(null);
-        const {
-            styles: styles2,
-            attributes: attributes2,
-            update: update2
-        } = usePopper$1(referenceElement.current, popperElement.current, {
-            modifiers: [sameWidthModifier],
-            placement: "bottom-start"
-        });
         const unpackedItems = React.useMemo(() => unpackSectionedList(props.items), [props.items]);
         const [pendingHighlight, setPendingHighlight] = React.useState(null);
         const [items, setItems] = React.useState(unpackedItems);
         const [inputValue, setInputValue] = React.useState((_b = (_a3 = props.selectedItem) === null || _a3 === void 0 ? void 0 : _a3.label) !== null && _b !== void 0 ? _b : "");
         const {
             selectedItem,
             isOpen,
@@ -54728,49 +53720,60 @@
             }
         }, [isOpen, pendingHighlight, setHighlightedIndex]);
         React.useEffect(() => {
             if (props.selectedItem === null) {
                 setInputValue("");
             }
         }, [props.selectedItem]);
-        React.useEffect(() => {
-            if (isOpen && update2) {
-                update2();
-            }
-        }, [isOpen, update2]);
+        const {
+            refs,
+            floatingStyles,
+            context: context2
+        } = useFloating({
+            open: isOpen,
+            placement: "bottom-start",
+            middleware: [flip$2(), shift$1(), matchWidthToReference(2)],
+            whileElementsMounted: isOpen ? autoUpdate : void 0
+        });
+        const role = useRole(context2, {
+            role: "listbox"
+        });
+        const {
+            getReferenceProps,
+            getFloatingProps
+        } = useInteractions([role]);
         const menuProps = getMenuProps();
         const setMenuRef = menuProps.ref;
-        delete menuProps.ref;
-        const setMenuReference = (value) => {
-            setMenuRef(value);
-            popperElement.current = value;
-        };
+        const setFloatingRef = refs.setFloating;
+        const mergedRefs = React.useCallback((node2) => {
+            setFloatingRef(node2);
+            setMenuRef(node2);
+        }, [setFloatingRef, setMenuRef]);
         return jsxRuntime.exports.jsxs(Wrapper$a, {
             className: props.className,
             isDisabled: props.disabled,
             isErrored: false,
             isOpen,
             style: props.style,
             children: [jsxRuntime.exports.jsxs(InputWrapper$4, {
                 disabled: props.disabled,
                 isOpen,
-                ref: referenceElement,
+                ref: refs.setReference,
                 children: [jsxRuntime.exports.jsx(Input$2, Object.assign({}, getInputProps({
                     value: inputValue
-                }))), jsxRuntime.exports.jsx(ChevronButton$1, Object.assign({}, getToggleButtonProps(), {
+                }), getReferenceProps())), jsxRuntime.exports.jsx(ChevronButton$1, Object.assign({}, getToggleButtonProps(), {
                     children: jsxRuntime.exports.jsx(Chevron$2, {
                         disabled: props.disabled,
                         isOpen
                     })
                 }))]
-            }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsxs(ListWrapper, Object.assign({}, menuProps, attributes2.popper, {
+            }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsxs(ListWrapper, Object.assign({}, menuProps, getFloatingProps(), {
+                ref: mergedRefs,
                 isOpen,
-                ref: setMenuReference,
-                style: Object.assign(Object.assign({}, styles2.popper), {
-                    width: parseFloat((_d = styles2.popper) === null || _d === void 0 ? void 0 : _d.width) + 2,
+                style: Object.assign(Object.assign({}, floatingStyles), {
                     zIndex: 9999
                 }),
                 children: [items.length > 0 && items.map((item, index2) => {
                     const itemProps = getItemProps({
                         index: index2,
                         item
                     });
@@ -61617,41 +60620,45 @@
         allColumns,
         allowColumnHiding,
         numVisibleColumns,
         resetResizing,
         setAllFilters,
         style: style2
     }) => {
-        const [optionsElement, setOptionsElement] = React.useState(null);
-        const [popperElement, setPopperElement] = React.useState(null);
-        const [showOptions, setShowOptions] = React.useState(false);
+        const [isOpen, setIsOpen] = React.useState(false);
+        const toggleOptions = React.useCallback(() => {
+            setIsOpen((prev) => !prev);
+        }, []);
+        const onOptionSelect = React.useCallback((option) => {
+            option.onClick();
+            setIsOpen(false);
+        }, []);
         const {
-            styles: styles2,
-            attributes: attributes2,
-            update: update2
-        } = usePopper$1(optionsElement, popperElement, {
-            placement: "left-end"
+            refs,
+            floatingStyles,
+            context: context2
+        } = useFloating({
+            open: isOpen,
+            onOpenChange: setIsOpen,
+            placement: "left-end",
+            middleware: [flip$2(), shift$1()],
+            whileElementsMounted: isOpen ? autoUpdate : void 0
         });
-        const toggleOptions = () => {
-            setShowOptions(!showOptions);
-        };
-        const onOptionSelect = (option) => {
-            option.onClick();
-        };
-        const clickOutsideOptionsHandler = () => {
-            if (showOptions) {
-                toggleOptions();
-            }
-        };
-        useOnClickOutside(popperElement, clickOutsideOptionsHandler);
-        React.useEffect(() => {
-            if (showOptions) {
-                update2();
-            }
-        }, [showOptions, update2]);
+        const interactions = useInteractions([
+            useClick(context2, {
+                event: "mousedown"
+            }),
+            useDismiss(context2, {
+                outsidePress: true,
+                outsidePressEvent: "mousedown"
+            }),
+            useRole(context2, {
+                role: "menu"
+            })
+        ]);
         const resetFunctions = React.useMemo(() => {
             const functions2 = {
                 items: [{
                     label: "Reset Column Widths",
                     onClick: resetResizing,
                     value: "resetResizing"
                 }, {
@@ -61683,30 +60690,31 @@
                     onClick: () => !(column.isVisible && numVisibleColumns === 1) ? column.toggleHidden() : null,
                     value: `${column.isVisible ? "hide" : "show"}${String(column.Header)}`
                 })),
                 label: "Columns"
             };
         }, [allColumns, allowColumnHiding, numVisibleColumns]);
         return jsxRuntime.exports.jsxs(HeaderOptions, {
-            ref: setOptionsElement,
+            ref: refs.setReference,
             children: [jsxRuntime.exports.jsx(HeaderOptionsIcon, {
                 icon: faEllipsisV,
                 onClick: toggleOptions
-            }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(OptionsDropdownList, Object.assign({}, attributes2.popper, {
-                isOpen: showOptions,
-                ref: setPopperElement,
-                style: Object.assign(Object.assign(Object.assign({}, styles2.popper), {
+            }), ReactDOM__default.default.createPortal(jsxRuntime.exports.jsx(OptionsDropdownList, Object.assign({}, interactions.getFloatingProps({
+                ref: refs.setFloating,
+                style: Object.assign(Object.assign(Object.assign({}, floatingStyles), {
                     maxHeight: 800,
                     minWidth: 150,
                     zIndex: 9999
-                }), style2),
+                }), style2)
+            }), {
+                isOpen,
                 children: jsxRuntime.exports.jsx(SectionedList, {
                     items: allowColumnHiding ? [resetFunctions, columnToggles] : [resetFunctions],
                     onSelect: onOptionSelect
-                })
+                }, isOpen ? "open" : "closed")
             })), document.body)]
         });
     };
     var __rest$7 = globalThis && globalThis.__rest || function(s2, e3) {
         var t2 = {};
         for (var p2 in s2)
             if (Object.prototype.hasOwnProperty.call(s2, p2) && e3.indexOf(p2) < 0)
@@ -69318,39 +68326,39 @@
             if (token.attrs[i2].name === attrName) {
                 return token.attrs[i2].value;
             }
         }
         return null;
     };
     var tokenizer = Tokenizer$4;
-    var html = {};
-    const NS$3 = html.NAMESPACES = {
+    var html$2 = {};
+    const NS$3 = html$2.NAMESPACES = {
         HTML: "http://www.w3.org/1999/xhtml",
         MATHML: "http://www.w3.org/1998/Math/MathML",
         SVG: "http://www.w3.org/2000/svg",
         XLINK: "http://www.w3.org/1999/xlink",
         XML: "http://www.w3.org/XML/1998/namespace",
         XMLNS: "http://www.w3.org/2000/xmlns/"
     };
-    html.ATTRS = {
+    html$2.ATTRS = {
         TYPE: "type",
         ACTION: "action",
         ENCODING: "encoding",
         PROMPT: "prompt",
         NAME: "name",
         COLOR: "color",
         FACE: "face",
         SIZE: "size"
     };
-    html.DOCUMENT_MODE = {
+    html$2.DOCUMENT_MODE = {
         NO_QUIRKS: "no-quirks",
         QUIRKS: "quirks",
         LIMITED_QUIRKS: "limited-quirks"
     };
-    const $$6 = html.TAG_NAMES = {
+    const $$6 = html$2.TAG_NAMES = {
         A: "a",
         ADDRESS: "address",
         ANNOTATION_XML: "annotation-xml",
         APPLET: "applet",
         AREA: "area",
         ARTICLE: "article",
         ASIDE: "aside",
@@ -69466,15 +68474,15 @@
         U: "u",
         UL: "ul",
         SVG: "svg",
         VAR: "var",
         WBR: "wbr",
         XMP: "xmp"
     };
-    html.SPECIAL_ELEMENTS = {
+    html$2.SPECIAL_ELEMENTS = {
         [NS$3.HTML]: {
             [$$6.ADDRESS]: true,
             [$$6.APPLET]: true,
             [$$6.AREA]: true,
             [$$6.ARTICLE]: true,
             [$$6.ASIDE]: true,
             [$$6.BASE]: true,
@@ -69564,15 +68572,15 @@
         },
         [NS$3.SVG]: {
             [$$6.TITLE]: true,
             [$$6.FOREIGN_OBJECT]: true,
             [$$6.DESC]: true
         }
     };
-    const HTML$4 = html;
+    const HTML$4 = html$2;
     const $$5 = HTML$4.TAG_NAMES;
     const NS$2 = HTML$4.NAMESPACES;
 
     function isImpliedEndTagRequired(tn) {
         switch (tn.length) {
             case 1:
                 return tn === $$5.P;
@@ -70244,15 +69252,15 @@
         }
     }
     var openElementStackMixin = LocationInfoOpenElementStackMixin$1;
     const Mixin$5 = mixin;
     const Tokenizer$2 = tokenizer;
     const LocationInfoTokenizerMixin$1 = tokenizerMixin$1;
     const LocationInfoOpenElementStackMixin = openElementStackMixin;
-    const HTML$3 = html;
+    const HTML$3 = html$2;
     const $$4 = HTML$3.TAG_NAMES;
     class LocationInfoParserMixin$1 extends Mixin$5 {
         constructor(parser2) {
             super(parser2);
             this.parser = parser2;
             this.treeAdapter = this.parser.treeAdapter;
             this.posTracker = null;
@@ -70502,15 +69510,15 @@
             };
         }
     }
     var parserMixin = ErrorReportingParserMixin$1;
     var _default = {};
     const {
         DOCUMENT_MODE: DOCUMENT_MODE$1
-    } = html;
+    } = html$2;
     _default.createDocument = function() {
         return {
             nodeName: "#document",
             mode: DOCUMENT_MODE$1.NO_QUIRKS,
             childNodes: []
         };
     };
@@ -70684,15 +69692,15 @@
             });
             return merged;
         }, /* @__PURE__ */ Object.create(null));
     };
     var doctype$2 = {};
     const {
         DOCUMENT_MODE
-    } = html;
+    } = html$2;
     const VALID_DOCTYPE_NAME = "html";
     const VALID_SYSTEM_ID = "about:legacy-compat";
     const QUIRKS_MODE_SYSTEM_ID = "http://www.ibm.com/data/dtd/v11/ibmxhtml1-transitional.dtd";
     const QUIRKS_MODE_PUBLIC_ID_PREFIXES = [
         "+//silmaril//dtd html pro v0r11 19970101//",
         "-//as//dtd html 3.0 aswedit + extensions//",
         "-//advasoft ltd//dtd html 3.0 aswedit + extensions//",
@@ -70814,15 +69822,15 @@
         if (systemId !== null) {
             str += " " + enquoteDoctypeId(systemId);
         }
         return str;
     };
     var foreignContent$1 = {};
     const Tokenizer$1 = tokenizer;
-    const HTML$2 = html;
+    const HTML$2 = html$2;
     const $$3 = HTML$2.TAG_NAMES;
     const NS$1 = HTML$2.NAMESPACES;
     const ATTRS$1 = HTML$2.ATTRS;
     const MIME_TYPES = {
         TEXT_HTML: "text/html",
         APPLICATION_XML: "application/xhtml+xml"
     };
@@ -71104,15 +70112,15 @@
     const Mixin = mixin;
     const defaultTreeAdapter = _default;
     const mergeOptions = mergeOptions$1;
     const doctype$1 = doctype$2;
     const foreignContent = foreignContent$1;
     const ERR = errorCodes;
     const unicode = unicode$3;
-    const HTML$1 = html;
+    const HTML$1 = html$2;
     const $$2 = HTML$1.TAG_NAMES;
     const NS = HTML$1.NAMESPACES;
     const ATTRS = HTML$1.ATTRS;
     const DEFAULT_OPTIONS = {
         scriptingEnabled: true,
         sourceCodeLocationInfo: false,
         onParseError: null,
@@ -73615,14 +72623,1126 @@
             return visitor(
                 node2,
                 parent ? parent.children.indexOf(node2) : null,
                 parent
             );
         }
     };
+    class Schema {
+        constructor(property, normal, space2) {
+            this.property = property;
+            this.normal = normal;
+            if (space2) {
+                this.space = space2;
+            }
+        }
+    }
+    Schema.prototype.property = {};
+    Schema.prototype.normal = {};
+    Schema.prototype.space = null;
+
+    function merge$1(definitions, space2) {
+        const property = {};
+        const normal = {};
+        let index2 = -1;
+        while (++index2 < definitions.length) {
+            Object.assign(property, definitions[index2].property);
+            Object.assign(normal, definitions[index2].normal);
+        }
+        return new Schema(property, normal, space2);
+    }
+
+    function normalize$1(value) {
+        return value.toLowerCase();
+    }
+    class Info {
+        constructor(property, attribute) {
+            this.property = property;
+            this.attribute = attribute;
+        }
+    }
+    Info.prototype.space = null;
+    Info.prototype.boolean = false;
+    Info.prototype.booleanish = false;
+    Info.prototype.overloadedBoolean = false;
+    Info.prototype.number = false;
+    Info.prototype.commaSeparated = false;
+    Info.prototype.spaceSeparated = false;
+    Info.prototype.commaOrSpaceSeparated = false;
+    Info.prototype.mustUseProperty = false;
+    Info.prototype.defined = false;
+    let powers = 0;
+    const boolean = increment();
+    const booleanish = increment();
+    const overloadedBoolean = increment();
+    const number$3 = increment();
+    const spaceSeparated = increment();
+    const commaSeparated = increment();
+    const commaOrSpaceSeparated = increment();
+
+    function increment() {
+        return 2 ** ++powers;
+    }
+    const types$1 = /* @__PURE__ */ Object.freeze( /* @__PURE__ */ Object.defineProperty({
+        __proto__: null,
+        boolean,
+        booleanish,
+        overloadedBoolean,
+        number: number$3,
+        spaceSeparated,
+        commaSeparated,
+        commaOrSpaceSeparated
+    }, Symbol.toStringTag, {
+        value: "Module"
+    }));
+    const checks = Object.keys(types$1);
+    class DefinedInfo extends Info {
+        constructor(property, attribute, mask, space2) {
+            let index2 = -1;
+            super(property, attribute);
+            mark(this, "space", space2);
+            if (typeof mask === "number") {
+                while (++index2 < checks.length) {
+                    const check = checks[index2];
+                    mark(this, checks[index2], (mask & types$1[check]) === types$1[check]);
+                }
+            }
+        }
+    }
+    DefinedInfo.prototype.defined = true;
+
+    function mark(values, key, value) {
+        if (value) {
+            values[key] = value;
+        }
+    }
+    const own$3 = {}.hasOwnProperty;
+
+    function create$1(definition2) {
+        const property = {};
+        const normal = {};
+        let prop;
+        for (prop in definition2.properties) {
+            if (own$3.call(definition2.properties, prop)) {
+                const value = definition2.properties[prop];
+                const info = new DefinedInfo(
+                    prop,
+                    definition2.transform(definition2.attributes || {}, prop),
+                    value,
+                    definition2.space
+                );
+                if (definition2.mustUseProperty && definition2.mustUseProperty.includes(prop)) {
+                    info.mustUseProperty = true;
+                }
+                property[prop] = info;
+                normal[normalize$1(prop)] = prop;
+                normal[normalize$1(info.attribute)] = prop;
+            }
+        }
+        return new Schema(property, normal, definition2.space);
+    }
+    const xlink = create$1({
+        space: "xlink",
+        transform(_2, prop) {
+            return "xlink:" + prop.slice(5).toLowerCase();
+        },
+        properties: {
+            xLinkActuate: null,
+            xLinkArcRole: null,
+            xLinkHref: null,
+            xLinkRole: null,
+            xLinkShow: null,
+            xLinkTitle: null,
+            xLinkType: null
+        }
+    });
+    const xml = create$1({
+        space: "xml",
+        transform(_2, prop) {
+            return "xml:" + prop.slice(3).toLowerCase();
+        },
+        properties: {
+            xmlLang: null,
+            xmlBase: null,
+            xmlSpace: null
+        }
+    });
+
+    function caseSensitiveTransform(attributes2, attribute) {
+        return attribute in attributes2 ? attributes2[attribute] : attribute;
+    }
+
+    function caseInsensitiveTransform(attributes2, property) {
+        return caseSensitiveTransform(attributes2, property.toLowerCase());
+    }
+    const xmlns = create$1({
+        space: "xmlns",
+        attributes: {
+            xmlnsxlink: "xmlns:xlink"
+        },
+        transform: caseInsensitiveTransform,
+        properties: {
+            xmlns: null,
+            xmlnsXLink: null
+        }
+    });
+    const aria = create$1({
+        transform(_2, prop) {
+            return prop === "role" ? prop : "aria-" + prop.slice(4).toLowerCase();
+        },
+        properties: {
+            ariaActiveDescendant: null,
+            ariaAtomic: booleanish,
+            ariaAutoComplete: null,
+            ariaBusy: booleanish,
+            ariaChecked: booleanish,
+            ariaColCount: number$3,
+            ariaColIndex: number$3,
+            ariaColSpan: number$3,
+            ariaControls: spaceSeparated,
+            ariaCurrent: null,
+            ariaDescribedBy: spaceSeparated,
+            ariaDetails: null,
+            ariaDisabled: booleanish,
+            ariaDropEffect: spaceSeparated,
+            ariaErrorMessage: null,
+            ariaExpanded: booleanish,
+            ariaFlowTo: spaceSeparated,
+            ariaGrabbed: booleanish,
+            ariaHasPopup: null,
+            ariaHidden: booleanish,
+            ariaInvalid: null,
+            ariaKeyShortcuts: null,
+            ariaLabel: null,
+            ariaLabelledBy: spaceSeparated,
+            ariaLevel: number$3,
+            ariaLive: null,
+            ariaModal: booleanish,
+            ariaMultiLine: booleanish,
+            ariaMultiSelectable: booleanish,
+            ariaOrientation: null,
+            ariaOwns: spaceSeparated,
+            ariaPlaceholder: null,
+            ariaPosInSet: number$3,
+            ariaPressed: booleanish,
+            ariaReadOnly: booleanish,
+            ariaRelevant: null,
+            ariaRequired: booleanish,
+            ariaRoleDescription: spaceSeparated,
+            ariaRowCount: number$3,
+            ariaRowIndex: number$3,
+            ariaRowSpan: number$3,
+            ariaSelected: booleanish,
+            ariaSetSize: number$3,
+            ariaSort: null,
+            ariaValueMax: number$3,
+            ariaValueMin: number$3,
+            ariaValueNow: number$3,
+            ariaValueText: null,
+            role: null
+        }
+    });
+    const html$1 = create$1({
+        space: "html",
+        attributes: {
+            acceptcharset: "accept-charset",
+            classname: "class",
+            htmlfor: "for",
+            httpequiv: "http-equiv"
+        },
+        transform: caseInsensitiveTransform,
+        mustUseProperty: ["checked", "multiple", "muted", "selected"],
+        properties: {
+            abbr: null,
+            accept: commaSeparated,
+            acceptCharset: spaceSeparated,
+            accessKey: spaceSeparated,
+            action: null,
+            allow: null,
+            allowFullScreen: boolean,
+            allowPaymentRequest: boolean,
+            allowUserMedia: boolean,
+            alt: null,
+            as: null,
+            async: boolean,
+            autoCapitalize: null,
+            autoComplete: spaceSeparated,
+            autoFocus: boolean,
+            autoPlay: boolean,
+            blocking: spaceSeparated,
+            capture: boolean,
+            charSet: null,
+            checked: boolean,
+            cite: null,
+            className: spaceSeparated,
+            cols: number$3,
+            colSpan: null,
+            content: null,
+            contentEditable: booleanish,
+            controls: boolean,
+            controlsList: spaceSeparated,
+            coords: number$3 | commaSeparated,
+            crossOrigin: null,
+            data: null,
+            dateTime: null,
+            decoding: null,
+            default: boolean,
+            defer: boolean,
+            dir: null,
+            dirName: null,
+            disabled: boolean,
+            download: overloadedBoolean,
+            draggable: booleanish,
+            encType: null,
+            enterKeyHint: null,
+            fetchPriority: null,
+            form: null,
+            formAction: null,
+            formEncType: null,
+            formMethod: null,
+            formNoValidate: boolean,
+            formTarget: null,
+            headers: spaceSeparated,
+            height: number$3,
+            hidden: boolean,
+            high: number$3,
+            href: null,
+            hrefLang: null,
+            htmlFor: spaceSeparated,
+            httpEquiv: spaceSeparated,
+            id: null,
+            imageSizes: null,
+            imageSrcSet: null,
+            inert: boolean,
+            inputMode: null,
+            integrity: null,
+            is: null,
+            isMap: boolean,
+            itemId: null,
+            itemProp: spaceSeparated,
+            itemRef: spaceSeparated,
+            itemScope: boolean,
+            itemType: spaceSeparated,
+            kind: null,
+            label: null,
+            lang: null,
+            language: null,
+            list: null,
+            loading: null,
+            loop: boolean,
+            low: number$3,
+            manifest: null,
+            max: null,
+            maxLength: number$3,
+            media: null,
+            method: null,
+            min: null,
+            minLength: number$3,
+            multiple: boolean,
+            muted: boolean,
+            name: null,
+            nonce: null,
+            noModule: boolean,
+            noValidate: boolean,
+            onAbort: null,
+            onAfterPrint: null,
+            onAuxClick: null,
+            onBeforeMatch: null,
+            onBeforePrint: null,
+            onBeforeToggle: null,
+            onBeforeUnload: null,
+            onBlur: null,
+            onCancel: null,
+            onCanPlay: null,
+            onCanPlayThrough: null,
+            onChange: null,
+            onClick: null,
+            onClose: null,
+            onContextLost: null,
+            onContextMenu: null,
+            onContextRestored: null,
+            onCopy: null,
+            onCueChange: null,
+            onCut: null,
+            onDblClick: null,
+            onDrag: null,
+            onDragEnd: null,
+            onDragEnter: null,
+            onDragExit: null,
+            onDragLeave: null,
+            onDragOver: null,
+            onDragStart: null,
+            onDrop: null,
+            onDurationChange: null,
+            onEmptied: null,
+            onEnded: null,
+            onError: null,
+            onFocus: null,
+            onFormData: null,
+            onHashChange: null,
+            onInput: null,
+            onInvalid: null,
+            onKeyDown: null,
+            onKeyPress: null,
+            onKeyUp: null,
+            onLanguageChange: null,
+            onLoad: null,
+            onLoadedData: null,
+            onLoadedMetadata: null,
+            onLoadEnd: null,
+            onLoadStart: null,
+            onMessage: null,
+            onMessageError: null,
+            onMouseDown: null,
+            onMouseEnter: null,
+            onMouseLeave: null,
+            onMouseMove: null,
+            onMouseOut: null,
+            onMouseOver: null,
+            onMouseUp: null,
+            onOffline: null,
+            onOnline: null,
+            onPageHide: null,
+            onPageShow: null,
+            onPaste: null,
+            onPause: null,
+            onPlay: null,
+            onPlaying: null,
+            onPopState: null,
+            onProgress: null,
+            onRateChange: null,
+            onRejectionHandled: null,
+            onReset: null,
+            onResize: null,
+            onScroll: null,
+            onScrollEnd: null,
+            onSecurityPolicyViolation: null,
+            onSeeked: null,
+            onSeeking: null,
+            onSelect: null,
+            onSlotChange: null,
+            onStalled: null,
+            onStorage: null,
+            onSubmit: null,
+            onSuspend: null,
+            onTimeUpdate: null,
+            onToggle: null,
+            onUnhandledRejection: null,
+            onUnload: null,
+            onVolumeChange: null,
+            onWaiting: null,
+            onWheel: null,
+            open: boolean,
+            optimum: number$3,
+            pattern: null,
+            ping: spaceSeparated,
+            placeholder: null,
+            playsInline: boolean,
+            popover: null,
+            popoverTarget: null,
+            popoverTargetAction: null,
+            poster: null,
+            preload: null,
+            readOnly: boolean,
+            referrerPolicy: null,
+            rel: spaceSeparated,
+            required: boolean,
+            reversed: boolean,
+            rows: number$3,
+            rowSpan: number$3,
+            sandbox: spaceSeparated,
+            scope: null,
+            scoped: boolean,
+            seamless: boolean,
+            selected: boolean,
+            shadowRootDelegatesFocus: boolean,
+            shadowRootMode: null,
+            shape: null,
+            size: number$3,
+            sizes: null,
+            slot: null,
+            span: number$3,
+            spellCheck: booleanish,
+            src: null,
+            srcDoc: null,
+            srcLang: null,
+            srcSet: null,
+            start: number$3,
+            step: null,
+            style: null,
+            tabIndex: number$3,
+            target: null,
+            title: null,
+            translate: null,
+            type: null,
+            typeMustMatch: boolean,
+            useMap: null,
+            value: booleanish,
+            width: number$3,
+            wrap: null,
+            align: null,
+            aLink: null,
+            archive: spaceSeparated,
+            axis: null,
+            background: null,
+            bgColor: null,
+            border: number$3,
+            borderColor: null,
+            bottomMargin: number$3,
+            cellPadding: null,
+            cellSpacing: null,
+            char: null,
+            charOff: null,
+            classId: null,
+            clear: null,
+            code: null,
+            codeBase: null,
+            codeType: null,
+            color: null,
+            compact: boolean,
+            declare: boolean,
+            event: null,
+            face: null,
+            frame: null,
+            frameBorder: null,
+            hSpace: number$3,
+            leftMargin: number$3,
+            link: null,
+            longDesc: null,
+            lowSrc: null,
+            marginHeight: number$3,
+            marginWidth: number$3,
+            noResize: boolean,
+            noHref: boolean,
+            noShade: boolean,
+            noWrap: boolean,
+            object: null,
+            profile: null,
+            prompt: null,
+            rev: null,
+            rightMargin: number$3,
+            rules: null,
+            scheme: null,
+            scrolling: booleanish,
+            standby: null,
+            summary: null,
+            text: null,
+            topMargin: number$3,
+            valueType: null,
+            version: null,
+            vAlign: null,
+            vLink: null,
+            vSpace: number$3,
+            allowTransparency: null,
+            autoCorrect: null,
+            autoSave: null,
+            disablePictureInPicture: boolean,
+            disableRemotePlayback: boolean,
+            prefix: null,
+            property: null,
+            results: number$3,
+            security: null,
+            unselectable: null
+        }
+    });
+    const svg$1 = create$1({
+        space: "svg",
+        attributes: {
+            accentHeight: "accent-height",
+            alignmentBaseline: "alignment-baseline",
+            arabicForm: "arabic-form",
+            baselineShift: "baseline-shift",
+            capHeight: "cap-height",
+            className: "class",
+            clipPath: "clip-path",
+            clipRule: "clip-rule",
+            colorInterpolation: "color-interpolation",
+            colorInterpolationFilters: "color-interpolation-filters",
+            colorProfile: "color-profile",
+            colorRendering: "color-rendering",
+            crossOrigin: "crossorigin",
+            dataType: "datatype",
+            dominantBaseline: "dominant-baseline",
+            enableBackground: "enable-background",
+            fillOpacity: "fill-opacity",
+            fillRule: "fill-rule",
+            floodColor: "flood-color",
+            floodOpacity: "flood-opacity",
+            fontFamily: "font-family",
+            fontSize: "font-size",
+            fontSizeAdjust: "font-size-adjust",
+            fontStretch: "font-stretch",
+            fontStyle: "font-style",
+            fontVariant: "font-variant",
+            fontWeight: "font-weight",
+            glyphName: "glyph-name",
+            glyphOrientationHorizontal: "glyph-orientation-horizontal",
+            glyphOrientationVertical: "glyph-orientation-vertical",
+            hrefLang: "hreflang",
+            horizAdvX: "horiz-adv-x",
+            horizOriginX: "horiz-origin-x",
+            horizOriginY: "horiz-origin-y",
+            imageRendering: "image-rendering",
+            letterSpacing: "letter-spacing",
+            lightingColor: "lighting-color",
+            markerEnd: "marker-end",
+            markerMid: "marker-mid",
+            markerStart: "marker-start",
+            navDown: "nav-down",
+            navDownLeft: "nav-down-left",
+            navDownRight: "nav-down-right",
+            navLeft: "nav-left",
+            navNext: "nav-next",
+            navPrev: "nav-prev",
+            navRight: "nav-right",
+            navUp: "nav-up",
+            navUpLeft: "nav-up-left",
+            navUpRight: "nav-up-right",
+            onAbort: "onabort",
+            onActivate: "onactivate",
+            onAfterPrint: "onafterprint",
+            onBeforePrint: "onbeforeprint",
+            onBegin: "onbegin",
+            onCancel: "oncancel",
+            onCanPlay: "oncanplay",
+            onCanPlayThrough: "oncanplaythrough",
+            onChange: "onchange",
+            onClick: "onclick",
+            onClose: "onclose",
+            onCopy: "oncopy",
+            onCueChange: "oncuechange",
+            onCut: "oncut",
+            onDblClick: "ondblclick",
+            onDrag: "ondrag",
+            onDragEnd: "ondragend",
+            onDragEnter: "ondragenter",
+            onDragExit: "ondragexit",
+            onDragLeave: "ondragleave",
+            onDragOver: "ondragover",
+            onDragStart: "ondragstart",
+            onDrop: "ondrop",
+            onDurationChange: "ondurationchange",
+            onEmptied: "onemptied",
+            onEnd: "onend",
+            onEnded: "onended",
+            onError: "onerror",
+            onFocus: "onfocus",
+            onFocusIn: "onfocusin",
+            onFocusOut: "onfocusout",
+            onHashChange: "onhashchange",
+            onInput: "oninput",
+            onInvalid: "oninvalid",
+            onKeyDown: "onkeydown",
+            onKeyPress: "onkeypress",
+            onKeyUp: "onkeyup",
+            onLoad: "onload",
+            onLoadedData: "onloadeddata",
+            onLoadedMetadata: "onloadedmetadata",
+            onLoadStart: "onloadstart",
+            onMessage: "onmessage",
+            onMouseDown: "onmousedown",
+            onMouseEnter: "onmouseenter",
+            onMouseLeave: "onmouseleave",
+            onMouseMove: "onmousemove",
+            onMouseOut: "onmouseout",
+            onMouseOver: "onmouseover",
+            onMouseUp: "onmouseup",
+            onMouseWheel: "onmousewheel",
+            onOffline: "onoffline",
+            onOnline: "ononline",
+            onPageHide: "onpagehide",
+            onPageShow: "onpageshow",
+            onPaste: "onpaste",
+            onPause: "onpause",
+            onPlay: "onplay",
+            onPlaying: "onplaying",
+            onPopState: "onpopstate",
+            onProgress: "onprogress",
+            onRateChange: "onratechange",
+            onRepeat: "onrepeat",
+            onReset: "onreset",
+            onResize: "onresize",
+            onScroll: "onscroll",
+            onSeeked: "onseeked",
+            onSeeking: "onseeking",
+            onSelect: "onselect",
+            onShow: "onshow",
+            onStalled: "onstalled",
+            onStorage: "onstorage",
+            onSubmit: "onsubmit",
+            onSuspend: "onsuspend",
+            onTimeUpdate: "ontimeupdate",
+            onToggle: "ontoggle",
+            onUnload: "onunload",
+            onVolumeChange: "onvolumechange",
+            onWaiting: "onwaiting",
+            onZoom: "onzoom",
+            overlinePosition: "overline-position",
+            overlineThickness: "overline-thickness",
+            paintOrder: "paint-order",
+            panose1: "panose-1",
+            pointerEvents: "pointer-events",
+            referrerPolicy: "referrerpolicy",
+            renderingIntent: "rendering-intent",
+            shapeRendering: "shape-rendering",
+            stopColor: "stop-color",
+            stopOpacity: "stop-opacity",
+            strikethroughPosition: "strikethrough-position",
+            strikethroughThickness: "strikethrough-thickness",
+            strokeDashArray: "stroke-dasharray",
+            strokeDashOffset: "stroke-dashoffset",
+            strokeLineCap: "stroke-linecap",
+            strokeLineJoin: "stroke-linejoin",
+            strokeMiterLimit: "stroke-miterlimit",
+            strokeOpacity: "stroke-opacity",
+            strokeWidth: "stroke-width",
+            tabIndex: "tabindex",
+            textAnchor: "text-anchor",
+            textDecoration: "text-decoration",
+            textRendering: "text-rendering",
+            transformOrigin: "transform-origin",
+            typeOf: "typeof",
+            underlinePosition: "underline-position",
+            underlineThickness: "underline-thickness",
+            unicodeBidi: "unicode-bidi",
+            unicodeRange: "unicode-range",
+            unitsPerEm: "units-per-em",
+            vAlphabetic: "v-alphabetic",
+            vHanging: "v-hanging",
+            vIdeographic: "v-ideographic",
+            vMathematical: "v-mathematical",
+            vectorEffect: "vector-effect",
+            vertAdvY: "vert-adv-y",
+            vertOriginX: "vert-origin-x",
+            vertOriginY: "vert-origin-y",
+            wordSpacing: "word-spacing",
+            writingMode: "writing-mode",
+            xHeight: "x-height",
+            playbackOrder: "playbackorder",
+            timelineBegin: "timelinebegin"
+        },
+        transform: caseSensitiveTransform,
+        properties: {
+            about: commaOrSpaceSeparated,
+            accentHeight: number$3,
+            accumulate: null,
+            additive: null,
+            alignmentBaseline: null,
+            alphabetic: number$3,
+            amplitude: number$3,
+            arabicForm: null,
+            ascent: number$3,
+            attributeName: null,
+            attributeType: null,
+            azimuth: number$3,
+            bandwidth: null,
+            baselineShift: null,
+            baseFrequency: null,
+            baseProfile: null,
+            bbox: null,
+            begin: null,
+            bias: number$3,
+            by: null,
+            calcMode: null,
+            capHeight: number$3,
+            className: spaceSeparated,
+            clip: null,
+            clipPath: null,
+            clipPathUnits: null,
+            clipRule: null,
+            color: null,
+            colorInterpolation: null,
+            colorInterpolationFilters: null,
+            colorProfile: null,
+            colorRendering: null,
+            content: null,
+            contentScriptType: null,
+            contentStyleType: null,
+            crossOrigin: null,
+            cursor: null,
+            cx: null,
+            cy: null,
+            d: null,
+            dataType: null,
+            defaultAction: null,
+            descent: number$3,
+            diffuseConstant: number$3,
+            direction: null,
+            display: null,
+            dur: null,
+            divisor: number$3,
+            dominantBaseline: null,
+            download: boolean,
+            dx: null,
+            dy: null,
+            edgeMode: null,
+            editable: null,
+            elevation: number$3,
+            enableBackground: null,
+            end: null,
+            event: null,
+            exponent: number$3,
+            externalResourcesRequired: null,
+            fill: null,
+            fillOpacity: number$3,
+            fillRule: null,
+            filter: null,
+            filterRes: null,
+            filterUnits: null,
+            floodColor: null,
+            floodOpacity: null,
+            focusable: null,
+            focusHighlight: null,
+            fontFamily: null,
+            fontSize: null,
+            fontSizeAdjust: null,
+            fontStretch: null,
+            fontStyle: null,
+            fontVariant: null,
+            fontWeight: null,
+            format: null,
+            fr: null,
+            from: null,
+            fx: null,
+            fy: null,
+            g1: commaSeparated,
+            g2: commaSeparated,
+            glyphName: commaSeparated,
+            glyphOrientationHorizontal: null,
+            glyphOrientationVertical: null,
+            glyphRef: null,
+            gradientTransform: null,
+            gradientUnits: null,
+            handler: null,
+            hanging: number$3,
+            hatchContentUnits: null,
+            hatchUnits: null,
+            height: null,
+            href: null,
+            hrefLang: null,
+            horizAdvX: number$3,
+            horizOriginX: number$3,
+            horizOriginY: number$3,
+            id: null,
+            ideographic: number$3,
+            imageRendering: null,
+            initialVisibility: null,
+            in: null,
+            in2: null,
+            intercept: number$3,
+            k: number$3,
+            k1: number$3,
+            k2: number$3,
+            k3: number$3,
+            k4: number$3,
+            kernelMatrix: commaOrSpaceSeparated,
+            kernelUnitLength: null,
+            keyPoints: null,
+            keySplines: null,
+            keyTimes: null,
+            kerning: null,
+            lang: null,
+            lengthAdjust: null,
+            letterSpacing: null,
+            lightingColor: null,
+            limitingConeAngle: number$3,
+            local: null,
+            markerEnd: null,
+            markerMid: null,
+            markerStart: null,
+            markerHeight: null,
+            markerUnits: null,
+            markerWidth: null,
+            mask: null,
+            maskContentUnits: null,
+            maskUnits: null,
+            mathematical: null,
+            max: null,
+            media: null,
+            mediaCharacterEncoding: null,
+            mediaContentEncodings: null,
+            mediaSize: number$3,
+            mediaTime: null,
+            method: null,
+            min: null,
+            mode: null,
+            name: null,
+            navDown: null,
+            navDownLeft: null,
+            navDownRight: null,
+            navLeft: null,
+            navNext: null,
+            navPrev: null,
+            navRight: null,
+            navUp: null,
+            navUpLeft: null,
+            navUpRight: null,
+            numOctaves: null,
+            observer: null,
+            offset: null,
+            onAbort: null,
+            onActivate: null,
+            onAfterPrint: null,
+            onBeforePrint: null,
+            onBegin: null,
+            onCancel: null,
+            onCanPlay: null,
+            onCanPlayThrough: null,
+            onChange: null,
+            onClick: null,
+            onClose: null,
+            onCopy: null,
+            onCueChange: null,
+            onCut: null,
+            onDblClick: null,
+            onDrag: null,
+            onDragEnd: null,
+            onDragEnter: null,
+            onDragExit: null,
+            onDragLeave: null,
+            onDragOver: null,
+            onDragStart: null,
+            onDrop: null,
+            onDurationChange: null,
+            onEmptied: null,
+            onEnd: null,
+            onEnded: null,
+            onError: null,
+            onFocus: null,
+            onFocusIn: null,
+            onFocusOut: null,
+            onHashChange: null,
+            onInput: null,
+            onInvalid: null,
+            onKeyDown: null,
+            onKeyPress: null,
+            onKeyUp: null,
+            onLoad: null,
+            onLoadedData: null,
+            onLoadedMetadata: null,
+            onLoadStart: null,
+            onMessage: null,
+            onMouseDown: null,
+            onMouseEnter: null,
+            onMouseLeave: null,
+            onMouseMove: null,
+            onMouseOut: null,
+            onMouseOver: null,
+            onMouseUp: null,
+            onMouseWheel: null,
+            onOffline: null,
+            onOnline: null,
+            onPageHide: null,
+            onPageShow: null,
+            onPaste: null,
+            onPause: null,
+            onPlay: null,
+            onPlaying: null,
+            onPopState: null,
+            onProgress: null,
+            onRateChange: null,
+            onRepeat: null,
+            onReset: null,
+            onResize: null,
+            onScroll: null,
+            onSeeked: null,
+            onSeeking: null,
+            onSelect: null,
+            onShow: null,
+            onStalled: null,
+            onStorage: null,
+            onSubmit: null,
+            onSuspend: null,
+            onTimeUpdate: null,
+            onToggle: null,
+            onUnload: null,
+            onVolumeChange: null,
+            onWaiting: null,
+            onZoom: null,
+            opacity: null,
+            operator: null,
+            order: null,
+            orient: null,
+            orientation: null,
+            origin: null,
+            overflow: null,
+            overlay: null,
+            overlinePosition: number$3,
+            overlineThickness: number$3,
+            paintOrder: null,
+            panose1: null,
+            path: null,
+            pathLength: number$3,
+            patternContentUnits: null,
+            patternTransform: null,
+            patternUnits: null,
+            phase: null,
+            ping: spaceSeparated,
+            pitch: null,
+            playbackOrder: null,
+            pointerEvents: null,
+            points: null,
+            pointsAtX: number$3,
+            pointsAtY: number$3,
+            pointsAtZ: number$3,
+            preserveAlpha: null,
+            preserveAspectRatio: null,
+            primitiveUnits: null,
+            propagate: null,
+            property: commaOrSpaceSeparated,
+            r: null,
+            radius: null,
+            referrerPolicy: null,
+            refX: null,
+            refY: null,
+            rel: commaOrSpaceSeparated,
+            rev: commaOrSpaceSeparated,
+            renderingIntent: null,
+            repeatCount: null,
+            repeatDur: null,
+            requiredExtensions: commaOrSpaceSeparated,
+            requiredFeatures: commaOrSpaceSeparated,
+            requiredFonts: commaOrSpaceSeparated,
+            requiredFormats: commaOrSpaceSeparated,
+            resource: null,
+            restart: null,
+            result: null,
+            rotate: null,
+            rx: null,
+            ry: null,
+            scale: null,
+            seed: null,
+            shapeRendering: null,
+            side: null,
+            slope: null,
+            snapshotTime: null,
+            specularConstant: number$3,
+            specularExponent: number$3,
+            spreadMethod: null,
+            spacing: null,
+            startOffset: null,
+            stdDeviation: null,
+            stemh: null,
+            stemv: null,
+            stitchTiles: null,
+            stopColor: null,
+            stopOpacity: null,
+            strikethroughPosition: number$3,
+            strikethroughThickness: number$3,
+            string: null,
+            stroke: null,
+            strokeDashArray: commaOrSpaceSeparated,
+            strokeDashOffset: null,
+            strokeLineCap: null,
+            strokeLineJoin: null,
+            strokeMiterLimit: number$3,
+            strokeOpacity: number$3,
+            strokeWidth: null,
+            style: null,
+            surfaceScale: number$3,
+            syncBehavior: null,
+            syncBehaviorDefault: null,
+            syncMaster: null,
+            syncTolerance: null,
+            syncToleranceDefault: null,
+            systemLanguage: commaOrSpaceSeparated,
+            tabIndex: number$3,
+            tableValues: null,
+            target: null,
+            targetX: number$3,
+            targetY: number$3,
+            textAnchor: null,
+            textDecoration: null,
+            textRendering: null,
+            textLength: null,
+            timelineBegin: null,
+            title: null,
+            transformBehavior: null,
+            type: null,
+            typeOf: commaOrSpaceSeparated,
+            to: null,
+            transform: null,
+            transformOrigin: null,
+            u1: null,
+            u2: null,
+            underlinePosition: number$3,
+            underlineThickness: number$3,
+            unicode: null,
+            unicodeBidi: null,
+            unicodeRange: null,
+            unitsPerEm: number$3,
+            values: null,
+            vAlphabetic: number$3,
+            vMathematical: number$3,
+            vectorEffect: null,
+            vHanging: number$3,
+            vIdeographic: number$3,
+            version: null,
+            vertAdvY: number$3,
+            vertOriginX: number$3,
+            vertOriginY: number$3,
+            viewBox: null,
+            viewTarget: null,
+            visibility: null,
+            width: null,
+            widths: null,
+            wordSpacing: null,
+            writingMode: null,
+            x: null,
+            x1: null,
+            x2: null,
+            xChannelSelector: null,
+            xHeight: number$3,
+            y: null,
+            y1: null,
+            y2: null,
+            yChannelSelector: null,
+            z: null,
+            zoomAndPan: null
+        }
+    });
+    const valid$1 = /^data[-\w.:]+$/i;
+    const dash = /-[a-z]/g;
+    const cap = /[A-Z]/g;
+
+    function find$3(schema, value) {
+        const normal = normalize$1(value);
+        let prop = value;
+        let Type2 = Info;
+        if (normal in schema.normal) {
+            return schema.property[schema.normal[normal]];
+        }
+        if (normal.length > 4 && normal.slice(0, 4) === "data" && valid$1.test(value)) {
+            if (value.charAt(4) === "-") {
+                const rest = value.slice(5).replace(dash, camelcase);
+                prop = "data" + rest.charAt(0).toUpperCase() + rest.slice(1);
+            } else {
+                const rest = value.slice(4);
+                if (!dash.test(rest)) {
+                    let dashes = rest.replace(cap, kebab);
+                    if (dashes.charAt(0) !== "-") {
+                        dashes = "-" + dashes;
+                    }
+                    value = "data" + dashes;
+                }
+            }
+            Type2 = DefinedInfo;
+        }
+        return new Type2(prop, value);
+    }
+
+    function kebab($0) {
+        return "-" + $0.toLowerCase();
+    }
+
+    function camelcase($0) {
+        return $0.charAt(1).toUpperCase();
+    }
+    const html = merge$1([xml, xlink, xmlns, aria, html$1], "html");
+    const svg = merge$1([xml, xlink, xmlns, aria, svg$1], "svg");
     const search = /[#.]/g;
 
     function parseSelector(selector2, defaultTagName) {
         const value = selector2 || "";
         const props = {};
         let start2 = 0;
         let previous2;
@@ -73782,15 +73902,15 @@
     }
 
     function parsePrimitive(info, name2, value) {
         if (typeof value === "string") {
             if (info.number && value && !Number.isNaN(Number(value))) {
                 return Number(value);
             }
-            if ((info.boolean || info.overloadedBoolean) && (value === "" || normalize$2(value) === normalize$2(name2))) {
+            if ((info.boolean || info.overloadedBoolean) && (value === "" || normalize$1(value) === normalize$1(name2))) {
                 return true;
             }
         }
         return value;
     }
 
     function style(value) {
@@ -73808,15 +73928,15 @@
         const result = {};
         let index2 = -1;
         while (++index2 < values.length) {
             result[values[index2].toLowerCase()] = values[index2];
         }
         return result;
     }
-    const h$1 = core$1(html$3, "div");
+    const h$1 = core$1(html, "div");
     const svgCaseSensitiveTagNames = [
         "altGlyph",
         "altGlyphDef",
         "altGlyphItem",
         "animateColor",
         "animateMotion",
         "animateTransform",
@@ -73920,15 +74040,15 @@
             file = options_;
             settings2 = {};
         } else {
             file = options_.file || void 0;
             settings2 = options_;
         }
         return one$2({
-                schema: settings2.space === "svg" ? svg : html$3,
+                schema: settings2.space === "svg" ? svg : html,
                 file,
                 verbose: settings2.verbose,
                 location: false
             },
             tree
         );
     }
@@ -74000,15 +74120,15 @@
             result[index2] = one$2(state, nodes[index2]);
         }
         return result;
     }
 
     function element$2(state, node2) {
         const schema = state.schema;
-        state.schema = node2.namespaceURI === webNamespaces.svg ? svg : html$3;
+        state.schema = node2.namespaceURI === webNamespaces.svg ? svg : html;
         let index2 = -1;
         const props = {};
         while (++index2 < node2.attrs.length) {
             const attribute = node2.attrs[index2];
             const name2 = (attribute.prefix ? attribute.prefix + ":" : "") + attribute.name;
             if (!own$1.call(proto, name2)) {
                 props[name2] = attribute.value;
@@ -74109,15 +74229,15 @@
             comment: comment$1,
             doctype
         }
     });
 
     function toParse5(tree, options) {
         const space2 = options && typeof options === "object" ? options.space : options;
-        return one$1(tree, space2 === "svg" ? svg : html$3);
+        return one$1(tree, space2 === "svg" ? svg : html);
     }
 
     function root$2(node2, schema) {
         const result = {
             nodeName: "#document",
             mode: (node2.data || {}).quirksMode ? "quirks" : "no-quirks",
             childNodes: []
@@ -234830,15 +234950,15 @@
                                     out[5] = 0;
                                     out[6] = 0;
                                     out[7] = 0;
                                     out[8] = 1;
                                     return out;
                                 }
 
-                                function create$2() {
+                                function create$22() {
                                     var out = new ARRAY_TYPE(16);
                                     if (ARRAY_TYPE != Float32Array) {
                                         out[1] = 0;
                                         out[2] = 0;
                                         out[3] = 0;
                                         out[4] = 0;
                                         out[6] = 0;
@@ -243650,15 +243770,15 @@
                                 exports4.clearTileCache = clearTileCache;
                                 exports4.clipLine = clipLine;
                                 exports4.clone = clone$1;
                                 exports4.clone$1 = clone2;
                                 exports4.clone$2 = clone$2;
                                 exports4.collisionCircleLayout = collisionCircleLayout;
                                 exports4.config = config2;
-                                exports4.create = create$2;
+                                exports4.create = create$22;
                                 exports4.create$1 = create$12;
                                 exports4.create$2 = create2;
                                 exports4.createCommonjsModule = createCommonjsModule2;
                                 exports4.createExpression = createExpression;
                                 exports4.createLayout = createLayout;
                                 exports4.createStyleLayer = createStyleLayer;
                                 exports4.cross = cross;
@@ -244714,15 +244834,15 @@
                                         coords[2 * i2 + 1] = getY2(points[i2]);
                                     }
                                     sortKD(ids, coords, nodeSize2, 0, ids.length - 1, 0);
                                 };
                                 KDBush.prototype.range = function range$1(minX, minY, maxX, maxY) {
                                     return range2(this.ids, this.coords, minX, minY, maxX, maxY, this.nodeSize);
                                 };
-                                KDBush.prototype.within = function within$12(x2, y2, r2) {
+                                KDBush.prototype.within = function within$1(x2, y2, r2) {
                                     return within2(this.ids, this.coords, x2, y2, r2, this.nodeSize);
                                 };
                                 var defaultOptions2 = {
                                     minZoom: 0,
                                     maxZoom: 16,
                                     minPoints: 2,
                                     radius: 40,
@@ -314534,138 +314654,138 @@
                 $rawCss: css2,
                 alt: "Matplotlib graph",
                 src: `data:image/svg+xml;base64,${props.figure}`,
                 style: style2
             }
         );
     }
-    var __defProp = Object.defineProperty;
-    var __getOwnPropSymbols = Object.getOwnPropertySymbols;
-    var __hasOwnProp = Object.prototype.hasOwnProperty;
-    var __propIsEnum = Object.prototype.propertyIsEnumerable;
-    var __defNormalProp = (obj, key, value) => key in obj ? __defProp(obj, key, {
+    var __defProp$1 = Object.defineProperty;
+    var __getOwnPropSymbols$1 = Object.getOwnPropertySymbols;
+    var __hasOwnProp$1 = Object.prototype.hasOwnProperty;
+    var __propIsEnum$1 = Object.prototype.propertyIsEnumerable;
+    var __defNormalProp$1 = (obj, key, value) => key in obj ? __defProp$1(obj, key, {
         enumerable: true,
         configurable: true,
         writable: true,
         value
     }) : obj[key] = value;
-    var __spreadValues = (a2, b2) => {
+    var __spreadValues$1 = (a2, b2) => {
         for (var prop in b2 || (b2 = {}))
-            if (__hasOwnProp.call(b2, prop))
-                __defNormalProp(a2, prop, b2[prop]);
-        if (__getOwnPropSymbols)
-            for (var prop of __getOwnPropSymbols(b2)) {
-                if (__propIsEnum.call(b2, prop))
-                    __defNormalProp(a2, prop, b2[prop]);
+            if (__hasOwnProp$1.call(b2, prop))
+                __defNormalProp$1(a2, prop, b2[prop]);
+        if (__getOwnPropSymbols$1)
+            for (var prop of __getOwnPropSymbols$1(b2)) {
+                if (__propIsEnum$1.call(b2, prop))
+                    __defNormalProp$1(a2, prop, b2[prop]);
             }
         return a2;
     };
-    var NOTHING = Symbol.for("immer-nothing");
-    var DRAFTABLE = Symbol.for("immer-draftable");
-    var DRAFT_STATE = Symbol.for("immer-state");
+    var NOTHING$1 = Symbol.for("immer-nothing");
+    var DRAFTABLE$1 = Symbol.for("immer-draftable");
+    var DRAFT_STATE$1 = Symbol.for("immer-state");
 
-    function die(error2, ...args) {
+    function die$1(error2, ...args) {
         throw new Error(
             `[Immer] minified error nr: ${error2}. Full error at: https://bit.ly/3cXEKWf`
         );
     }
-    var getPrototypeOf = Object.getPrototypeOf;
+    var getPrototypeOf$1 = Object.getPrototypeOf;
 
-    function isDraft(value) {
-        return !!value && !!value[DRAFT_STATE];
+    function isDraft$1(value) {
+        return !!value && !!value[DRAFT_STATE$1];
     }
 
-    function isDraftable(value) {
+    function isDraftable$1(value) {
         var _a3;
         if (!value)
             return false;
-        return isPlainObject$2(value) || Array.isArray(value) || !!value[DRAFTABLE] || !!((_a3 = value.constructor) == null ? void 0 : _a3[DRAFTABLE]) || isMap$3(value) || isSet$3(value);
+        return isPlainObject$3(value) || Array.isArray(value) || !!value[DRAFTABLE$1] || !!((_a3 = value.constructor) == null ? void 0 : _a3[DRAFTABLE$1]) || isMap$4(value) || isSet$4(value);
     }
-    var objectCtorString = Object.prototype.constructor.toString();
+    var objectCtorString$1 = Object.prototype.constructor.toString();
 
-    function isPlainObject$2(value) {
+    function isPlainObject$3(value) {
         if (!value || typeof value !== "object")
             return false;
-        const proto2 = getPrototypeOf(value);
+        const proto2 = getPrototypeOf$1(value);
         if (proto2 === null) {
             return true;
         }
         const Ctor = Object.hasOwnProperty.call(proto2, "constructor") && proto2.constructor;
         if (Ctor === Object)
             return true;
-        return typeof Ctor == "function" && Function.toString.call(Ctor) === objectCtorString;
+        return typeof Ctor == "function" && Function.toString.call(Ctor) === objectCtorString$1;
     }
 
-    function each(obj, iter2) {
-        if (getArchtype(obj) === 0) {
+    function each$1(obj, iter2) {
+        if (getArchtype$1(obj) === 0) {
             Reflect.ownKeys(obj).forEach((key) => {
                 iter2(key, obj[key], obj);
             });
         } else {
             obj.forEach((entry, index2) => iter2(index2, entry, obj));
         }
     }
 
-    function getArchtype(thing) {
-        const state = thing[DRAFT_STATE];
-        return state ? state.type_ : Array.isArray(thing) ? 1 : isMap$3(thing) ? 2 : isSet$3(thing) ? 3 : 0;
+    function getArchtype$1(thing) {
+        const state = thing[DRAFT_STATE$1];
+        return state ? state.type_ : Array.isArray(thing) ? 1 : isMap$4(thing) ? 2 : isSet$4(thing) ? 3 : 0;
     }
 
-    function has$4(thing, prop) {
-        return getArchtype(thing) === 2 ? thing.has(prop) : Object.prototype.hasOwnProperty.call(thing, prop);
+    function has$5(thing, prop) {
+        return getArchtype$1(thing) === 2 ? thing.has(prop) : Object.prototype.hasOwnProperty.call(thing, prop);
     }
 
-    function set$3(thing, propOrOldValue, value) {
-        const t2 = getArchtype(thing);
+    function set$4(thing, propOrOldValue, value) {
+        const t2 = getArchtype$1(thing);
         if (t2 === 2)
             thing.set(propOrOldValue, value);
         else if (t2 === 3) {
             thing.add(value);
         } else
             thing[propOrOldValue] = value;
     }
 
-    function is(x2, y2) {
+    function is$1(x2, y2) {
         if (x2 === y2) {
             return x2 !== 0 || 1 / x2 === 1 / y2;
         } else {
             return x2 !== x2 && y2 !== y2;
         }
     }
 
-    function isMap$3(target) {
+    function isMap$4(target) {
         return target instanceof Map;
     }
 
-    function isSet$3(target) {
+    function isSet$4(target) {
         return target instanceof Set;
     }
 
-    function latest(state) {
+    function latest$1(state) {
         return state.copy_ || state.base_;
     }
 
-    function shallowCopy(base2, strict) {
-        if (isMap$3(base2)) {
+    function shallowCopy$1(base2, strict) {
+        if (isMap$4(base2)) {
             return new Map(base2);
         }
-        if (isSet$3(base2)) {
+        if (isSet$4(base2)) {
             return new Set(base2);
         }
         if (Array.isArray(base2))
             return Array.prototype.slice.call(base2);
-        if (!strict && isPlainObject$2(base2)) {
-            if (!getPrototypeOf(base2)) {
+        if (!strict && isPlainObject$3(base2)) {
+            if (!getPrototypeOf$1(base2)) {
                 const obj = /* @__PURE__ */ Object.create(null);
                 return Object.assign(obj, base2);
             }
-            return __spreadValues({}, base2);
+            return __spreadValues$1({}, base2);
         }
         const descriptors = Object.getOwnPropertyDescriptors(base2);
-        delete descriptors[DRAFT_STATE];
+        delete descriptors[DRAFT_STATE$1];
         let keys2 = Reflect.ownKeys(descriptors);
         for (let i2 = 0; i2 < keys2.length; i2++) {
             const key = keys2[i2];
             const desc = descriptors[key];
             if (desc.writable === false) {
                 desc.writable = true;
                 desc.configurable = true;
@@ -314674,418 +314794,418 @@
                 descriptors[key] = {
                     configurable: true,
                     writable: true,
                     enumerable: desc.enumerable,
                     value: base2[key]
                 };
         }
-        return Object.create(getPrototypeOf(base2), descriptors);
+        return Object.create(getPrototypeOf$1(base2), descriptors);
     }
 
-    function freeze(obj, deep = false) {
-        if (isFrozen(obj) || isDraft(obj) || !isDraftable(obj))
+    function freeze$1(obj, deep = false) {
+        if (isFrozen$1(obj) || isDraft$1(obj) || !isDraftable$1(obj))
             return obj;
-        if (getArchtype(obj) > 1) {
-            obj.set = obj.add = obj.clear = obj.delete = dontMutateFrozenCollections;
+        if (getArchtype$1(obj) > 1) {
+            obj.set = obj.add = obj.clear = obj.delete = dontMutateFrozenCollections$1;
         }
         Object.freeze(obj);
         if (deep)
-            Object.entries(obj).forEach(([key, value]) => freeze(value, true));
+            Object.entries(obj).forEach(([key, value]) => freeze$1(value, true));
         return obj;
     }
 
-    function dontMutateFrozenCollections() {
-        die(2);
+    function dontMutateFrozenCollections$1() {
+        die$1(2);
     }
 
-    function isFrozen(obj) {
+    function isFrozen$1(obj) {
         return Object.isFrozen(obj);
     }
-    var plugins = {};
+    var plugins$1 = {};
 
-    function getPlugin(pluginKey) {
-        const plugin = plugins[pluginKey];
+    function getPlugin$1(pluginKey) {
+        const plugin = plugins$1[pluginKey];
         if (!plugin) {
-            die(0, pluginKey);
+            die$1(0, pluginKey);
         }
         return plugin;
     }
-    var currentScope;
+    var currentScope$1;
 
-    function getCurrentScope() {
-        return currentScope;
+    function getCurrentScope$1() {
+        return currentScope$1;
     }
 
-    function createScope(parent_, immer_) {
+    function createScope$1(parent_, immer_) {
         return {
             drafts_: [],
             parent_,
             immer_,
             canAutoFreeze_: true,
             unfinalizedDrafts_: 0
         };
     }
 
-    function usePatchesInScope(scope2, patchListener) {
+    function usePatchesInScope$1(scope2, patchListener) {
         if (patchListener) {
-            getPlugin("Patches");
+            getPlugin$1("Patches");
             scope2.patches_ = [];
             scope2.inversePatches_ = [];
             scope2.patchListener_ = patchListener;
         }
     }
 
-    function revokeScope(scope2) {
-        leaveScope(scope2);
-        scope2.drafts_.forEach(revokeDraft);
+    function revokeScope$1(scope2) {
+        leaveScope$1(scope2);
+        scope2.drafts_.forEach(revokeDraft$1);
         scope2.drafts_ = null;
     }
 
-    function leaveScope(scope2) {
-        if (scope2 === currentScope) {
-            currentScope = scope2.parent_;
+    function leaveScope$1(scope2) {
+        if (scope2 === currentScope$1) {
+            currentScope$1 = scope2.parent_;
         }
     }
 
-    function enterScope(immer2) {
-        return currentScope = createScope(currentScope, immer2);
+    function enterScope$1(immer2) {
+        return currentScope$1 = createScope$1(currentScope$1, immer2);
     }
 
-    function revokeDraft(draft) {
-        const state = draft[DRAFT_STATE];
+    function revokeDraft$1(draft) {
+        const state = draft[DRAFT_STATE$1];
         if (state.type_ === 0 || state.type_ === 1)
             state.revoke_();
         else
             state.revoked_ = true;
     }
 
-    function processResult(result, scope2) {
+    function processResult$1(result, scope2) {
         scope2.unfinalizedDrafts_ = scope2.drafts_.length;
         const baseDraft = scope2.drafts_[0];
         const isReplaced = result !== void 0 && result !== baseDraft;
         if (isReplaced) {
-            if (baseDraft[DRAFT_STATE].modified_) {
-                revokeScope(scope2);
-                die(4);
+            if (baseDraft[DRAFT_STATE$1].modified_) {
+                revokeScope$1(scope2);
+                die$1(4);
             }
-            if (isDraftable(result)) {
-                result = finalize(scope2, result);
+            if (isDraftable$1(result)) {
+                result = finalize$1(scope2, result);
                 if (!scope2.parent_)
-                    maybeFreeze(scope2, result);
+                    maybeFreeze$1(scope2, result);
             }
             if (scope2.patches_) {
-                getPlugin("Patches").generateReplacementPatches_(
-                    baseDraft[DRAFT_STATE].base_,
+                getPlugin$1("Patches").generateReplacementPatches_(
+                    baseDraft[DRAFT_STATE$1].base_,
                     result,
                     scope2.patches_,
                     scope2.inversePatches_
                 );
             }
         } else {
-            result = finalize(scope2, baseDraft, []);
+            result = finalize$1(scope2, baseDraft, []);
         }
-        revokeScope(scope2);
+        revokeScope$1(scope2);
         if (scope2.patches_) {
             scope2.patchListener_(scope2.patches_, scope2.inversePatches_);
         }
-        return result !== NOTHING ? result : void 0;
+        return result !== NOTHING$1 ? result : void 0;
     }
 
-    function finalize(rootScope, value, path2) {
-        if (isFrozen(value))
+    function finalize$1(rootScope, value, path2) {
+        if (isFrozen$1(value))
             return value;
-        const state = value[DRAFT_STATE];
+        const state = value[DRAFT_STATE$1];
         if (!state) {
-            each(
+            each$1(
                 value,
-                (key, childValue) => finalizeProperty(rootScope, state, value, key, childValue, path2)
+                (key, childValue) => finalizeProperty$1(rootScope, state, value, key, childValue, path2)
             );
             return value;
         }
         if (state.scope_ !== rootScope)
             return value;
         if (!state.modified_) {
-            maybeFreeze(rootScope, state.base_, true);
+            maybeFreeze$1(rootScope, state.base_, true);
             return state.base_;
         }
         if (!state.finalized_) {
             state.finalized_ = true;
             state.scope_.unfinalizedDrafts_--;
             const result = state.copy_;
             let resultEach = result;
             let isSet2 = false;
             if (state.type_ === 3) {
                 resultEach = new Set(result);
                 result.clear();
                 isSet2 = true;
             }
-            each(
+            each$1(
                 resultEach,
-                (key, childValue) => finalizeProperty(rootScope, state, result, key, childValue, path2, isSet2)
+                (key, childValue) => finalizeProperty$1(rootScope, state, result, key, childValue, path2, isSet2)
             );
-            maybeFreeze(rootScope, result, false);
+            maybeFreeze$1(rootScope, result, false);
             if (path2 && rootScope.patches_) {
-                getPlugin("Patches").generatePatches_(
+                getPlugin$1("Patches").generatePatches_(
                     state,
                     path2,
                     rootScope.patches_,
                     rootScope.inversePatches_
                 );
             }
         }
         return state.copy_;
     }
 
-    function finalizeProperty(rootScope, parentState, targetObject, prop, childValue, rootPath, targetIsSet) {
-        if (isDraft(childValue)) {
-            const path2 = rootPath && parentState && parentState.type_ !== 3 && !has$4(parentState.assigned_, prop) ? rootPath.concat(prop) : void 0;
-            const res = finalize(rootScope, childValue, path2);
-            set$3(targetObject, prop, res);
-            if (isDraft(res)) {
+    function finalizeProperty$1(rootScope, parentState, targetObject, prop, childValue, rootPath, targetIsSet) {
+        if (isDraft$1(childValue)) {
+            const path2 = rootPath && parentState && parentState.type_ !== 3 && !has$5(parentState.assigned_, prop) ? rootPath.concat(prop) : void 0;
+            const res = finalize$1(rootScope, childValue, path2);
+            set$4(targetObject, prop, res);
+            if (isDraft$1(res)) {
                 rootScope.canAutoFreeze_ = false;
             } else
                 return;
         } else if (targetIsSet) {
             targetObject.add(childValue);
         }
-        if (isDraftable(childValue) && !isFrozen(childValue)) {
+        if (isDraftable$1(childValue) && !isFrozen$1(childValue)) {
             if (!rootScope.immer_.autoFreeze_ && rootScope.unfinalizedDrafts_ < 1) {
                 return;
             }
-            finalize(rootScope, childValue);
+            finalize$1(rootScope, childValue);
             if ((!parentState || !parentState.scope_.parent_) && typeof prop !== "symbol" && Object.prototype.propertyIsEnumerable.call(targetObject, prop))
-                maybeFreeze(rootScope, childValue);
+                maybeFreeze$1(rootScope, childValue);
         }
     }
 
-    function maybeFreeze(scope2, value, deep = false) {
+    function maybeFreeze$1(scope2, value, deep = false) {
         if (!scope2.parent_ && scope2.immer_.autoFreeze_ && scope2.canAutoFreeze_) {
-            freeze(value, deep);
+            freeze$1(value, deep);
         }
     }
 
-    function createProxyProxy(base2, parent) {
+    function createProxyProxy$1(base2, parent) {
         const isArray2 = Array.isArray(base2);
         const state = {
             type_: isArray2 ? 1 : 0,
-            scope_: parent ? parent.scope_ : getCurrentScope(),
+            scope_: parent ? parent.scope_ : getCurrentScope$1(),
             modified_: false,
             finalized_: false,
             assigned_: {},
             parent_: parent,
             base_: base2,
             draft_: null,
             copy_: null,
             revoke_: null,
             isManual_: false
         };
         let target = state;
-        let traps = objectTraps;
+        let traps = objectTraps$1;
         if (isArray2) {
             target = [state];
-            traps = arrayTraps;
+            traps = arrayTraps$1;
         }
         const {
             revoke,
             proxy
         } = Proxy.revocable(target, traps);
         state.draft_ = proxy;
         state.revoke_ = revoke;
         return proxy;
     }
-    var objectTraps = {
+    var objectTraps$1 = {
         get(state, prop) {
-            if (prop === DRAFT_STATE)
+            if (prop === DRAFT_STATE$1)
                 return state;
-            const source = latest(state);
-            if (!has$4(source, prop)) {
-                return readPropFromProto(state, source, prop);
+            const source = latest$1(state);
+            if (!has$5(source, prop)) {
+                return readPropFromProto$1(state, source, prop);
             }
             const value = source[prop];
-            if (state.finalized_ || !isDraftable(value)) {
+            if (state.finalized_ || !isDraftable$1(value)) {
                 return value;
             }
-            if (value === peek(state.base_, prop)) {
-                prepareCopy(state);
-                return state.copy_[prop] = createProxy(value, state);
+            if (value === peek$1(state.base_, prop)) {
+                prepareCopy$1(state);
+                return state.copy_[prop] = createProxy$1(value, state);
             }
             return value;
         },
         has(state, prop) {
-            return prop in latest(state);
+            return prop in latest$1(state);
         },
         ownKeys(state) {
-            return Reflect.ownKeys(latest(state));
+            return Reflect.ownKeys(latest$1(state));
         },
         set(state, prop, value) {
-            const desc = getDescriptorFromProto(latest(state), prop);
+            const desc = getDescriptorFromProto$1(latest$1(state), prop);
             if (desc == null ? void 0 : desc.set) {
                 desc.set.call(state.draft_, value);
                 return true;
             }
             if (!state.modified_) {
-                const current2 = peek(latest(state), prop);
-                const currentState = current2 == null ? void 0 : current2[DRAFT_STATE];
+                const current2 = peek$1(latest$1(state), prop);
+                const currentState = current2 == null ? void 0 : current2[DRAFT_STATE$1];
                 if (currentState && currentState.base_ === value) {
                     state.copy_[prop] = value;
                     state.assigned_[prop] = false;
                     return true;
                 }
-                if (is(value, current2) && (value !== void 0 || has$4(state.base_, prop)))
+                if (is$1(value, current2) && (value !== void 0 || has$5(state.base_, prop)))
                     return true;
-                prepareCopy(state);
-                markChanged(state);
+                prepareCopy$1(state);
+                markChanged$1(state);
             }
             if (state.copy_[prop] === value && (value !== void 0 || prop in state.copy_) || Number.isNaN(value) && Number.isNaN(state.copy_[prop]))
                 return true;
             state.copy_[prop] = value;
             state.assigned_[prop] = true;
             return true;
         },
         deleteProperty(state, prop) {
-            if (peek(state.base_, prop) !== void 0 || prop in state.base_) {
+            if (peek$1(state.base_, prop) !== void 0 || prop in state.base_) {
                 state.assigned_[prop] = false;
-                prepareCopy(state);
-                markChanged(state);
+                prepareCopy$1(state);
+                markChanged$1(state);
             } else {
                 delete state.assigned_[prop];
             }
             if (state.copy_) {
                 delete state.copy_[prop];
             }
             return true;
         },
         getOwnPropertyDescriptor(state, prop) {
-            const owner = latest(state);
+            const owner = latest$1(state);
             const desc = Reflect.getOwnPropertyDescriptor(owner, prop);
             if (!desc)
                 return desc;
             return {
                 writable: true,
                 configurable: state.type_ !== 1 || prop !== "length",
                 enumerable: desc.enumerable,
                 value: owner[prop]
             };
         },
         defineProperty() {
-            die(11);
+            die$1(11);
         },
         getPrototypeOf(state) {
-            return getPrototypeOf(state.base_);
+            return getPrototypeOf$1(state.base_);
         },
         setPrototypeOf() {
-            die(12);
+            die$1(12);
         }
     };
-    var arrayTraps = {};
-    each(objectTraps, (key, fn2) => {
-        arrayTraps[key] = function() {
+    var arrayTraps$1 = {};
+    each$1(objectTraps$1, (key, fn2) => {
+        arrayTraps$1[key] = function() {
             arguments[0] = arguments[0][0];
             return fn2.apply(this, arguments);
         };
     });
-    arrayTraps.deleteProperty = function(state, prop) {
-        return arrayTraps.set.call(this, state, prop, void 0);
+    arrayTraps$1.deleteProperty = function(state, prop) {
+        return arrayTraps$1.set.call(this, state, prop, void 0);
     };
-    arrayTraps.set = function(state, prop, value) {
-        return objectTraps.set.call(this, state[0], prop, value, state[0]);
+    arrayTraps$1.set = function(state, prop, value) {
+        return objectTraps$1.set.call(this, state[0], prop, value, state[0]);
     };
 
-    function peek(draft, prop) {
-        const state = draft[DRAFT_STATE];
-        const source = state ? latest(state) : draft;
+    function peek$1(draft, prop) {
+        const state = draft[DRAFT_STATE$1];
+        const source = state ? latest$1(state) : draft;
         return source[prop];
     }
 
-    function readPropFromProto(state, source, prop) {
+    function readPropFromProto$1(state, source, prop) {
         var _a3;
-        const desc = getDescriptorFromProto(source, prop);
+        const desc = getDescriptorFromProto$1(source, prop);
         return desc ? `value` in desc ? desc.value : (_a3 = desc.get) == null ? void 0 : _a3.call(state.draft_) : void 0;
     }
 
-    function getDescriptorFromProto(source, prop) {
+    function getDescriptorFromProto$1(source, prop) {
         if (!(prop in source))
             return void 0;
-        let proto2 = getPrototypeOf(source);
+        let proto2 = getPrototypeOf$1(source);
         while (proto2) {
             const desc = Object.getOwnPropertyDescriptor(proto2, prop);
             if (desc)
                 return desc;
-            proto2 = getPrototypeOf(proto2);
+            proto2 = getPrototypeOf$1(proto2);
         }
         return void 0;
     }
 
-    function markChanged(state) {
+    function markChanged$1(state) {
         if (!state.modified_) {
             state.modified_ = true;
             if (state.parent_) {
-                markChanged(state.parent_);
+                markChanged$1(state.parent_);
             }
         }
     }
 
-    function prepareCopy(state) {
+    function prepareCopy$1(state) {
         if (!state.copy_) {
-            state.copy_ = shallowCopy(
+            state.copy_ = shallowCopy$1(
                 state.base_,
                 state.scope_.immer_.useStrictShallowCopy_
             );
         }
     }
-    var Immer2 = class {
+    var Immer2$1 = class {
         constructor(config2) {
             this.autoFreeze_ = true;
             this.useStrictShallowCopy_ = false;
             this.produce = (base2, recipe, patchListener) => {
                 if (typeof base2 === "function" && typeof recipe !== "function") {
                     const defaultBase = recipe;
                     recipe = base2;
                     const self2 = this;
                     return function curriedProduce(base22 = defaultBase, ...args) {
                         return self2.produce(base22, (draft) => recipe.call(this, draft, ...args));
                     };
                 }
                 if (typeof recipe !== "function")
-                    die(6);
+                    die$1(6);
                 if (patchListener !== void 0 && typeof patchListener !== "function")
-                    die(7);
+                    die$1(7);
                 let result;
-                if (isDraftable(base2)) {
-                    const scope2 = enterScope(this);
-                    const proxy = createProxy(base2, void 0);
+                if (isDraftable$1(base2)) {
+                    const scope2 = enterScope$1(this);
+                    const proxy = createProxy$1(base2, void 0);
                     let hasError = true;
                     try {
                         result = recipe(proxy);
                         hasError = false;
                     } finally {
                         if (hasError)
-                            revokeScope(scope2);
+                            revokeScope$1(scope2);
                         else
-                            leaveScope(scope2);
+                            leaveScope$1(scope2);
                     }
-                    usePatchesInScope(scope2, patchListener);
-                    return processResult(result, scope2);
+                    usePatchesInScope$1(scope2, patchListener);
+                    return processResult$1(result, scope2);
                 } else if (!base2 || typeof base2 !== "object") {
                     result = recipe(base2);
                     if (result === void 0)
                         result = base2;
-                    if (result === NOTHING)
+                    if (result === NOTHING$1)
                         result = void 0;
                     if (this.autoFreeze_)
-                        freeze(result, true);
+                        freeze$1(result, true);
                     if (patchListener) {
                         const p2 = [];
                         const ip = [];
-                        getPlugin("Patches").generateReplacementPatches_(base2, result, p2, ip);
+                        getPlugin$1("Patches").generateReplacementPatches_(base2, result, p2, ip);
                         patchListener(p2, ip);
                     }
                     return result;
                 } else
-                    die(1, base2);
+                    die$1(1, base2);
             };
             this.produceWithPatches = (base2, recipe) => {
                 if (typeof base2 === "function") {
                     return (state, ...args) => this.produceWithPatches(state, (draft) => base2(draft, ...args));
                 }
                 let patches, inversePatches;
                 const result = this.produce(base2, recipe, (p2, ip) => {
@@ -315096,33 +315216,33 @@
             };
             if (typeof(config2 == null ? void 0 : config2.autoFreeze) === "boolean")
                 this.setAutoFreeze(config2.autoFreeze);
             if (typeof(config2 == null ? void 0 : config2.useStrictShallowCopy) === "boolean")
                 this.setUseStrictShallowCopy(config2.useStrictShallowCopy);
         }
         createDraft(base2) {
-            if (!isDraftable(base2))
-                die(8);
-            if (isDraft(base2))
-                base2 = current(base2);
-            const scope2 = enterScope(this);
-            const proxy = createProxy(base2, void 0);
-            proxy[DRAFT_STATE].isManual_ = true;
-            leaveScope(scope2);
+            if (!isDraftable$1(base2))
+                die$1(8);
+            if (isDraft$1(base2))
+                base2 = current$1(base2);
+            const scope2 = enterScope$1(this);
+            const proxy = createProxy$1(base2, void 0);
+            proxy[DRAFT_STATE$1].isManual_ = true;
+            leaveScope$1(scope2);
             return proxy;
         }
         finishDraft(draft, patchListener) {
-            const state = draft && draft[DRAFT_STATE];
+            const state = draft && draft[DRAFT_STATE$1];
             if (!state || !state.isManual_)
-                die(9);
+                die$1(9);
             const {
                 scope_: scope2
             } = state;
-            usePatchesInScope(scope2, patchListener);
-            return processResult(void 0, scope2);
+            usePatchesInScope$1(scope2, patchListener);
+            return processResult$1(void 0, scope2);
         }
         setAutoFreeze(value) {
             this.autoFreeze_ = value;
         }
         setUseStrictShallowCopy(value) {
             this.useStrictShallowCopy_ = value;
         }
@@ -315134,69 +315254,69 @@
                     base2 = patch2.value;
                     break;
                 }
             }
             if (i2 > -1) {
                 patches = patches.slice(i2 + 1);
             }
-            const applyPatchesImpl = getPlugin("Patches").applyPatches_;
-            if (isDraft(base2)) {
+            const applyPatchesImpl = getPlugin$1("Patches").applyPatches_;
+            if (isDraft$1(base2)) {
                 return applyPatchesImpl(base2, patches);
             }
             return this.produce(
                 base2,
                 (draft) => applyPatchesImpl(draft, patches)
             );
         }
     };
 
-    function createProxy(value, parent) {
-        const draft = isMap$3(value) ? getPlugin("MapSet").proxyMap_(value, parent) : isSet$3(value) ? getPlugin("MapSet").proxySet_(value, parent) : createProxyProxy(value, parent);
-        const scope2 = parent ? parent.scope_ : getCurrentScope();
+    function createProxy$1(value, parent) {
+        const draft = isMap$4(value) ? getPlugin$1("MapSet").proxyMap_(value, parent) : isSet$4(value) ? getPlugin$1("MapSet").proxySet_(value, parent) : createProxyProxy$1(value, parent);
+        const scope2 = parent ? parent.scope_ : getCurrentScope$1();
         scope2.drafts_.push(draft);
         return draft;
     }
 
-    function current(value) {
-        if (!isDraft(value))
-            die(10, value);
-        return currentImpl(value);
+    function current$1(value) {
+        if (!isDraft$1(value))
+            die$1(10, value);
+        return currentImpl$1(value);
     }
 
-    function currentImpl(value) {
-        if (!isDraftable(value) || isFrozen(value))
+    function currentImpl$1(value) {
+        if (!isDraftable$1(value) || isFrozen$1(value))
             return value;
-        const state = value[DRAFT_STATE];
+        const state = value[DRAFT_STATE$1];
         let copy2;
         if (state) {
             if (!state.modified_)
                 return state.base_;
             state.finalized_ = true;
-            copy2 = shallowCopy(value, state.scope_.immer_.useStrictShallowCopy_);
+            copy2 = shallowCopy$1(value, state.scope_.immer_.useStrictShallowCopy_);
         } else {
-            copy2 = shallowCopy(value, true);
+            copy2 = shallowCopy$1(value, true);
         }
-        each(copy2, (key, childValue) => {
-            set$3(copy2, key, currentImpl(childValue));
+        each$1(copy2, (key, childValue) => {
+            set$4(copy2, key, currentImpl$1(childValue));
         });
         if (state) {
             state.finalized_ = false;
         }
         return copy2;
     }
-    var immer = new Immer2();
-    var produce = immer.produce;
-    immer.produceWithPatches.bind(
-        immer
+    var immer$1 = new Immer2$1();
+    var produce$1 = immer$1.produce;
+    immer$1.produceWithPatches.bind(
+        immer$1
     );
-    immer.setAutoFreeze.bind(immer);
-    immer.setUseStrictShallowCopy.bind(immer);
-    immer.applyPatches.bind(immer);
-    immer.createDraft.bind(immer);
-    immer.finishDraft.bind(immer);
+    immer$1.setAutoFreeze.bind(immer$1);
+    immer$1.setUseStrictShallowCopy.bind(immer$1);
+    immer$1.applyPatches.bind(immer$1);
+    immer$1.createDraft.bind(immer$1);
+    immer$1.finishDraft.bind(immer$1);
     const ColumnSelect = styled__default.default(Select$1)`
     flex-basis: 15rem;
 `;
     const FilterLabel = styled__default.default.span`
     flex-basis: 50px;
 `;
     const AddFilterButton = styled__default.default(Button$3)`
@@ -315265,41 +315385,41 @@
         }, [columns]);
         const columnMap = React.useMemo(() => {
             return columns.reduce((acc, c2) => acc.set(c2.name, c2.type), /* @__PURE__ */ new Map());
         }, [columns]);
         const updateFilter = React.useMemo(
             () => debounce_1$1((id2, property, value) => {
                 setFilters(
-                    (currentFilters) => produce(currentFilters, (draft) => {
+                    (currentFilters) => produce$1(currentFilters, (draft) => {
                         const filter2 = draft.find((d2) => d2.__id === id2);
                         filter2[property] = value;
                     })
                 );
             }, 500),
             []
         );
 
         function addFilter() {
             setFilters(
-                produce(filters2, (draft) => {
+                produce$1(filters2, (draft) => {
                     draft.push({
                         __id: nanoid(),
                         column: null,
                         from_date: "",
                         range: "",
                         to_date: "",
                         values: ""
                     });
                 })
             );
         }
 
         function removeFilter(id2) {
             setFilters(
-                produce(filters2, (draft) => {
+                produce$1(filters2, (draft) => {
                     const fIndex = draft.findIndex((f2) => f2.__id === id2);
                     draft.splice(fIndex, 1);
                 })
             );
         }
         return /* @__PURE__ */ React__default.default.createElement(SlicerFilterWrapper, {
             style: {
@@ -315470,18 +315590,18 @@
                         return t2;
                 return;
             }
             if (callback != null && typeof callback !== "function")
                 throw new Error("invalid callback: " + callback);
             while (++i2 < n2) {
                 if (t2 = (typename = T2[i2]).type)
-                    _2[t2] = set$2(_2[t2], typename.name, callback);
+                    _2[t2] = set$3(_2[t2], typename.name, callback);
                 else if (callback == null)
                     for (t2 in _2)
-                        _2[t2] = set$2(_2[t2], typename.name, null);
+                        _2[t2] = set$3(_2[t2], typename.name, null);
             }
             return this;
         },
         copy: function() {
             var copy2 = {},
                 _2 = this._;
             for (var t2 in _2)
@@ -315509,15 +315629,15 @@
         for (var i2 = 0, n2 = type2.length, c2; i2 < n2; ++i2) {
             if ((c2 = type2[i2]).name === name2) {
                 return c2.value;
             }
         }
     }
 
-    function set$2(type2, name2, callback) {
+    function set$3(type2, name2, callback) {
         for (var i2 = 0, n2 = type2.length; i2 < n2; ++i2) {
             if (type2[i2].name === name2) {
                 type2[i2] = noop$4, type2 = type2.slice(0, i2).concat(type2.slice(i2 + 1));
                 break;
             }
         }
         if (callback != null)
@@ -317165,15 +317285,15 @@
     function init$1(node2, id2) {
         var schedule2 = get$2(node2, id2);
         if (schedule2.state > CREATED)
             throw new Error("too late; already scheduled");
         return schedule2;
     }
 
-    function set$1(node2, id2) {
+    function set$2(node2, id2) {
         var schedule2 = get$2(node2, id2);
         if (schedule2.state > STARTED)
             throw new Error("too late; already running");
         return schedule2;
     }
 
     function get$2(node2, id2) {
@@ -317289,15 +317409,15 @@
             interrupt(this, name2);
         });
     }
 
     function tweenRemove(id2, name2) {
         var tween0, tween1;
         return function() {
-            var schedule2 = set$1(this, id2),
+            var schedule2 = set$2(this, id2),
                 tween = schedule2.tween;
             if (tween !== tween0) {
                 tween1 = tween0 = tween;
                 for (var i2 = 0, n2 = tween1.length; i2 < n2; ++i2) {
                     if (tween1[i2].name === name2) {
                         tween1 = tween1.slice();
                         tween1.splice(i2, 1);
@@ -317310,15 +317430,15 @@
     }
 
     function tweenFunction(id2, name2, value) {
         var tween0, tween1;
         if (typeof value !== "function")
             throw new Error();
         return function() {
-            var schedule2 = set$1(this, id2),
+            var schedule2 = set$2(this, id2),
                 tween = schedule2.tween;
             if (tween !== tween0) {
                 tween1 = (tween0 = tween).slice();
                 for (var t2 = {
                         name: name2,
                         value
                     }, i2 = 0, n2 = tween1.length; i2 < n2; ++i2) {
@@ -317348,15 +317468,15 @@
         }
         return this.each((value == null ? tweenRemove : tweenFunction)(id2, name2, value));
     }
 
     function tweenValue(transition, name2, value) {
         var id2 = transition._id;
         transition.each(function() {
-            var schedule2 = set$1(this, id2);
+            var schedule2 = set$2(this, id2);
             (schedule2.value || (schedule2.value = {}))[name2] = value.apply(this, arguments);
         });
         return function(node2) {
             return get$2(node2, id2).value[name2];
         };
     }
 
@@ -317493,49 +317613,49 @@
     function transition_delay(value) {
         var id2 = this._id;
         return arguments.length ? this.each((typeof value === "function" ? delayFunction : delayConstant)(id2, value)) : get$2(this.node(), id2).delay;
     }
 
     function durationFunction(id2, value) {
         return function() {
-            set$1(this, id2).duration = +value.apply(this, arguments);
+            set$2(this, id2).duration = +value.apply(this, arguments);
         };
     }
 
     function durationConstant(id2, value) {
         return value = +value,
             function() {
-                set$1(this, id2).duration = value;
+                set$2(this, id2).duration = value;
             };
     }
 
     function transition_duration(value) {
         var id2 = this._id;
         return arguments.length ? this.each((typeof value === "function" ? durationFunction : durationConstant)(id2, value)) : get$2(this.node(), id2).duration;
     }
 
     function easeConstant(id2, value) {
         if (typeof value !== "function")
             throw new Error();
         return function() {
-            set$1(this, id2).ease = value;
+            set$2(this, id2).ease = value;
         };
     }
 
     function transition_ease(value) {
         var id2 = this._id;
         return arguments.length ? this.each(easeConstant(id2, value)) : get$2(this.node(), id2).ease;
     }
 
     function easeVarying(id2, value) {
         return function() {
             var v3 = value.apply(this, arguments);
             if (typeof v3 !== "function")
                 throw new Error();
-            set$1(this, id2).ease = v3;
+            set$2(this, id2).ease = v3;
         };
     }
 
     function transition_easeVarying(value) {
         if (typeof value !== "function")
             throw new Error();
         return this.each(easeVarying(this._id, value));
@@ -317576,15 +317696,15 @@
             if (i2 >= 0)
                 t2 = t2.slice(0, i2);
             return !t2 || t2 === "start";
         });
     }
 
     function onFunction(id2, name2, listener2) {
-        var on0, on1, sit = start(name2) ? init$1 : set$1;
+        var on0, on1, sit = start(name2) ? init$1 : set$2;
         return function() {
             var schedule2 = sit(this, id2),
                 on = schedule2.on;
             if (on !== on0)
                 (on1 = (on0 = on).copy()).on(name2, listener2);
             schedule2.on = on1;
         };
@@ -317691,15 +317811,15 @@
     }
 
     function styleMaybeRemove(id2, name2) {
         var on0, on1, listener0, key = "style." + name2,
             event2 = "end." + key,
             remove2;
         return function() {
-            var schedule2 = set$1(this, id2),
+            var schedule2 = set$2(this, id2),
                 on = schedule2.on,
                 listener2 = schedule2.value[key] == null ? remove2 || (remove2 = styleRemove(name2)) : void 0;
             if (on !== on0 || listener0 !== listener2)
                 (on1 = (on0 = on).copy()).on(event2, listener0 = listener2);
             schedule2.on = on1;
         };
     }
@@ -317817,15 +317937,15 @@
                 end2 = {
                     value: function() {
                         if (--size2 === 0)
                             resolve2();
                     }
                 };
             that.each(function() {
-                var schedule2 = set$1(this, id2),
+                var schedule2 = set$2(this, id2),
                     on = schedule2.on;
                 if (on !== on0) {
                     on1 = (on0 = on).copy();
                     on1._.cancel.push(cancel);
                     on1._.interrupt.push(cancel);
                     on1._.end.push(end2);
                 }
@@ -338741,14 +338861,40 @@
             label: "from",
             detail: "import",
             type: "keyword"
         })
     ];
     const globalCompletion = /* @__PURE__ */ ifNotIn(dontComplete, /* @__PURE__ */ completeFromList( /* @__PURE__ */ globals.concat(snippets)));
 
+    function innerBody(context2) {
+        let {
+            node: node2,
+            pos
+        } = context2;
+        let lineIndent = context2.lineIndent(pos, -1);
+        let found = null;
+        for (;;) {
+            let before = node2.childBefore(pos);
+            if (!before) {
+                break;
+            } else if (before.name == "Comment") {
+                pos = before.from;
+            } else if (before.name == "Body") {
+                if (context2.baseIndentFor(before) + context2.unit <= lineIndent)
+                    found = before;
+                node2 = before;
+            } else if (before.type.is("Statement")) {
+                node2 = before;
+            } else {
+                break;
+            }
+        }
+        return found;
+    }
+
     function indentBody(context2, node2) {
         let base2 = context2.baseIndentFor(node2);
         let line = context2.lineAt(context2.pos, -1),
             to2 = line.from + line.text.length;
         if (/^\s*($|#)/.test(line.text) && context2.node.to < to2 + 100 && !/\S/.test(context2.state.sliceDoc(to2, context2.node.to)) && context2.lineIndent(context2.pos, -1) <= base2)
             return null;
         if (/^\s*(else:|elif |except |finally:)/.test(context2.textAfter) && context2.lineIndent(context2.pos, -1) > base2)
@@ -338759,15 +338905,16 @@
         name: "python",
         parser: /* @__PURE__ */ parser$1.configure({
             props: [
                 /* @__PURE__ */
                 indentNodeProp.add({
                     Body: (context2) => {
                         var _a3;
-                        return (_a3 = indentBody(context2, context2.node)) !== null && _a3 !== void 0 ? _a3 : context2.continue();
+                        let inner = innerBody(context2);
+                        return (_a3 = indentBody(context2, inner || context2.node)) !== null && _a3 !== void 0 ? _a3 : context2.continue();
                     },
                     IfStatement: (cx) => /^\s*(else:|elif )/.test(cx.textAfter) ? cx.baseIndent : cx.continue(),
                     "ForStatement WhileStatement": (cx) => /^\s*else:/.test(cx.textAfter) ? cx.baseIndent : cx.continue(),
                     TryStatement: (cx) => /^\s*(except |finally:|else:)/.test(cx.textAfter) ? cx.baseIndent : cx.continue(),
                     "TupleExpression ComprehensionExpression ParamList ArgList ParenthesizedExpression": /* @__PURE__ */ delimitedIndent({
                         closing: ")"
                     }),
@@ -338775,30 +338922,17 @@
                         closing: "}"
                     }),
                     "ArrayExpression ArrayComprehensionExpression": /* @__PURE__ */ delimitedIndent({
                         closing: "]"
                     }),
                     "String FormatString": () => null,
                     Script: (context2) => {
-                        if (context2.pos + /\s*/.exec(context2.textAfter)[0].length >= context2.node.to) {
-                            let endBody = null;
-                            for (let cur = context2.node, to2 = cur.to;;) {
-                                cur = cur.lastChild;
-                                if (!cur || cur.to != to2)
-                                    break;
-                                if (cur.type.name == "Body")
-                                    endBody = cur;
-                            }
-                            if (endBody) {
-                                let bodyIndent = indentBody(context2, endBody);
-                                if (bodyIndent != null)
-                                    return bodyIndent;
-                            }
-                        }
-                        return context2.continue();
+                        var _a3;
+                        let inner = innerBody(context2);
+                        return (_a3 = inner && indentBody(context2, inner)) !== null && _a3 !== void 0 ? _a3 : context2.continue();
                     }
                 }),
                 /* @__PURE__ */
                 foldNodeProp.add({
                     "ArrayExpression DictionaryExpression SetExpression TupleExpression": foldInside,
                     Body: (node2, state) => ({
                         from: node2.from + 1,
@@ -340097,20 +340231,20 @@
 
     margin: 1rem;
 
     border-radius: 0.4rem;
 `;
     const ChatButton = styled__default.default.button`
     position: absolute;
-    right: 1rem;
-    bottom: 1rem;
+    right: 0.5rem;
+    bottom: 0.5rem;
 
-    width: 2rem;
-    height: 2rem;
-    padding-top: 0.45rem;
+    width: 32px;
+    height: 32px;
+    padding: 7px 6px;
 
     color: ${(props) => props.theme.colors.background};
 
     background-color: ${(props) => props.theme.colors.primary};
     border: none;
     border-radius: 2rem;
 
@@ -340235,17 +340369,17 @@
                     activeUser: parseUserData(userData)
                 }
             )
         ), /* @__PURE__ */ React__namespace.createElement(ChatButton, {
             onClick: onClickChatButton
         }, /* @__PURE__ */ React__namespace.createElement("svg", {
             fill: "none",
-            height: "32",
-            viewBox: "0 0 52 52",
-            width: "32",
+            height: "20",
+            viewBox: "0 0 32 32",
+            width: "20",
             xmlns: "http://www.w3.org/2000/svg"
         }, /* @__PURE__ */ React__namespace.createElement("rect", {
             fill: "none",
             height: "24",
             rx: "3",
             width: "30",
             x: "1",
@@ -347327,28 +347461,28 @@
         return $replace.call(str, sepRegex, "$&_");
     }
     var utilInspect = require$$0;
     var inspectCustom = utilInspect.custom;
     var inspectSymbol = isSymbol$1(inspectCustom) ? inspectCustom : null;
     var objectInspect = function inspect_(obj, options, depth, seen) {
         var opts = options || {};
-        if (has$3(opts, "quoteStyle") && (opts.quoteStyle !== "single" && opts.quoteStyle !== "double")) {
+        if (has$4(opts, "quoteStyle") && (opts.quoteStyle !== "single" && opts.quoteStyle !== "double")) {
             throw new TypeError('option "quoteStyle" must be "single" or "double"');
         }
-        if (has$3(opts, "maxStringLength") && (typeof opts.maxStringLength === "number" ? opts.maxStringLength < 0 && opts.maxStringLength !== Infinity : opts.maxStringLength !== null)) {
+        if (has$4(opts, "maxStringLength") && (typeof opts.maxStringLength === "number" ? opts.maxStringLength < 0 && opts.maxStringLength !== Infinity : opts.maxStringLength !== null)) {
             throw new TypeError('option "maxStringLength", if provided, must be a positive integer, Infinity, or `null`');
         }
-        var customInspect = has$3(opts, "customInspect") ? opts.customInspect : true;
+        var customInspect = has$4(opts, "customInspect") ? opts.customInspect : true;
         if (typeof customInspect !== "boolean" && customInspect !== "symbol") {
             throw new TypeError("option \"customInspect\", if provided, must be `true`, `false`, or `'symbol'`");
         }
-        if (has$3(opts, "indent") && opts.indent !== null && opts.indent !== "	" && !(parseInt(opts.indent, 10) === opts.indent && opts.indent > 0)) {
+        if (has$4(opts, "indent") && opts.indent !== null && opts.indent !== "	" && !(parseInt(opts.indent, 10) === opts.indent && opts.indent > 0)) {
             throw new TypeError('option "indent" must be "\\t", an integer > 0, or `null`');
         }
-        if (has$3(opts, "numericSeparator") && typeof opts.numericSeparator !== "boolean") {
+        if (has$4(opts, "numericSeparator") && typeof opts.numericSeparator !== "boolean") {
             throw new TypeError('option "numericSeparator", if provided, must be `true` or `false`');
         }
         var numericSeparator = opts.numericSeparator;
         if (typeof obj === "undefined") {
             return "undefined";
         }
         if (obj === null) {
@@ -347390,15 +347524,15 @@
                 seen = $arrSlice.call(seen);
                 seen.push(from);
             }
             if (noIndent) {
                 var newOpts = {
                     depth: opts.depth
                 };
-                if (has$3(opts, "quoteStyle")) {
+                if (has$4(opts, "quoteStyle")) {
                     newOpts.quoteStyle = opts.quoteStyle;
                 }
                 return inspect_(value, newOpts, depth + 1, seen);
             }
             return inspect_(value, opts, depth + 1, seen);
         }
         if (typeof obj === "function" && !isRegExp$1(obj)) {
@@ -347448,24 +347582,24 @@
                 return utilInspect(obj, {
                     depth: maxDepth - depth
                 });
             } else if (customInspect !== "symbol" && typeof obj.inspect === "function") {
                 return obj.inspect();
             }
         }
-        if (isMap$2(obj)) {
+        if (isMap$3(obj)) {
             var mapParts = [];
             if (mapForEach) {
                 mapForEach.call(obj, function(value, key) {
                     mapParts.push(inspect2(key, obj, true) + " => " + inspect2(value, obj));
                 });
             }
             return collectionOf("Map", mapSize$1.call(obj), mapParts, indent2);
         }
-        if (isSet$2(obj)) {
+        if (isSet$3(obj)) {
             var setParts = [];
             if (setForEach) {
                 setForEach.call(obj, function(value) {
                     setParts.push(inspect2(value, obj));
                 });
             }
             return collectionOf("Set", setSize.call(obj), setParts, indent2);
@@ -347579,15 +347713,15 @@
         } catch (e3) {}
         return false;
     }
     var hasOwn = Object.prototype.hasOwnProperty || function(key) {
         return key in this;
     };
 
-    function has$3(obj, key) {
+    function has$4(obj, key) {
         return hasOwn.call(obj, key);
     }
 
     function toStr(obj) {
         return objectToString$1.call(obj);
     }
 
@@ -347610,15 +347744,15 @@
             if (xs[i2] === x2) {
                 return i2;
             }
         }
         return -1;
     }
 
-    function isMap$2(x2) {
+    function isMap$3(x2) {
         if (!mapSize$1 || !x2 || typeof x2 !== "object") {
             return false;
         }
         try {
             mapSize$1.call(x2);
             try {
                 setSize.call(x2);
@@ -347653,15 +347787,15 @@
         try {
             weakRefDeref.call(x2);
             return true;
         } catch (e3) {}
         return false;
     }
 
-    function isSet$2(x2) {
+    function isSet$3(x2) {
         if (!setSize || !x2 || typeof x2 !== "object") {
             return false;
         }
         try {
             setSize.call(x2);
             try {
                 mapSize$1.call(x2);
@@ -347771,27 +347905,27 @@
 
     function arrObjKeys(obj, inspect2) {
         var isArr = isArray$5(obj);
         var xs = [];
         if (isArr) {
             xs.length = obj.length;
             for (var i2 = 0; i2 < obj.length; i2++) {
-                xs[i2] = has$3(obj, i2) ? inspect2(obj[i2], obj) : "";
+                xs[i2] = has$4(obj, i2) ? inspect2(obj[i2], obj) : "";
             }
         }
         var syms = typeof gOPS === "function" ? gOPS(obj) : [];
         var symMap;
         if (hasShammedSymbols) {
             symMap = {};
             for (var k2 = 0; k2 < syms.length; k2++) {
                 symMap["$" + syms[k2]] = syms[k2];
             }
         }
         for (var key in obj) {
-            if (!has$3(obj, key)) {
+            if (!has$4(obj, key)) {
                 continue;
             }
             if (isArr && String(Number(key)) === key && key < obj.length) {
                 continue;
             }
             if (hasShammedSymbols && symMap["$" + key] instanceof Symbol) {
                 continue;
@@ -347935,15 +348069,15 @@
                 return String(value);
             }
         },
         RFC1738: Format.RFC1738,
         RFC3986: Format.RFC3986
     };
     var formats$3 = formats$4;
-    var has$2 = Object.prototype.hasOwnProperty;
+    var has$3 = Object.prototype.hasOwnProperty;
     var isArray$4 = Array.isArray;
     var hexTable = function() {
         var array2 = [];
         for (var i2 = 0; i2 < 256; ++i2) {
             array2.push("%" + ((i2 < 16 ? "0" : "") + i2.toString(16)).toUpperCase());
         }
         return array2;
@@ -347976,15 +348110,15 @@
         if (!source) {
             return target;
         }
         if (typeof source !== "object") {
             if (isArray$4(target)) {
                 target.push(source);
             } else if (target && typeof target === "object") {
-                if (options && (options.plainObjects || options.allowPrototypes) || !has$2.call(Object.prototype, source)) {
+                if (options && (options.plainObjects || options.allowPrototypes) || !has$3.call(Object.prototype, source)) {
                     target[source] = true;
                 }
             } else {
                 return [target, source];
             }
             return target;
         }
@@ -347993,30 +348127,30 @@
         }
         var mergeTarget = target;
         if (isArray$4(target) && !isArray$4(source)) {
             mergeTarget = arrayToObject(target, options);
         }
         if (isArray$4(target) && isArray$4(source)) {
             source.forEach(function(item, i2) {
-                if (has$2.call(target, i2)) {
+                if (has$3.call(target, i2)) {
                     var targetItem = target[i2];
                     if (targetItem && typeof targetItem === "object" && item && typeof item === "object") {
                         target[i2] = merge2(targetItem, item, options);
                     } else {
                         target.push(item);
                     }
                 } else {
                     target[i2] = item;
                 }
             });
             return target;
         }
         return Object.keys(source).reduce(function(acc, key) {
             var value = source[key];
-            if (has$2.call(acc, key)) {
+            if (has$3.call(acc, key)) {
                 acc[key] = merge2(acc[key], value, options);
             } else {
                 acc[key] = value;
             }
             return acc;
         }, mergeTarget);
     };
@@ -348143,15 +348277,15 @@
         isRegExp,
         maybeMap,
         merge
     };
     var getSideChannel = sideChannel;
     var utils$1 = utils$2;
     var formats$2 = formats$4;
-    var has$1 = Object.prototype.hasOwnProperty;
+    var has$2 = Object.prototype.hasOwnProperty;
     var arrayPrefixGenerators = {
         brackets: function brackets(prefix) {
             return prefix + "[]";
         },
         comma: "comma",
         indices: function indices2(prefix, key) {
             return prefix + "[" + key + "]";
@@ -348308,15 +348442,15 @@
         }
         var charset = opts.charset || defaults$l.charset;
         if (typeof opts.charset !== "undefined" && opts.charset !== "utf-8" && opts.charset !== "iso-8859-1") {
             throw new TypeError("The charset option must be either utf-8, iso-8859-1, or undefined");
         }
         var format2 = formats$2["default"];
         if (typeof opts.format !== "undefined") {
-            if (!has$1.call(formats$2.formatters, opts.format)) {
+            if (!has$2.call(formats$2.formatters, opts.format)) {
                 throw new TypeError("Unknown format option provided.");
             }
             format2 = opts.format;
         }
         var formatter = formats$2.formatters[format2];
         var filter2 = defaults$l.filter;
         if (typeof opts.filter === "function" || isArray$3(opts.filter)) {
@@ -348415,15 +348549,15 @@
             } else {
                 prefix += "utf8=%E2%9C%93&";
             }
         }
         return joined.length > 0 ? prefix + joined : "";
     };
     var utils = utils$2;
-    var has = Object.prototype.hasOwnProperty;
+    var has$1 = Object.prototype.hasOwnProperty;
     var isArray$2 = Array.isArray;
     var defaults$k = {
         allowDots: false,
         allowEmptyArrays: false,
         allowPrototypes: false,
         allowSparse: false,
         arrayLimit: 20,
@@ -348500,15 +348634,15 @@
             }
             if (val && options.interpretNumericEntities && charset === "iso-8859-1") {
                 val = interpretNumericEntities(val);
             }
             if (part.indexOf("[]=") > -1) {
                 val = isArray$2(val) ? [val] : val;
             }
-            var existing = has.call(obj, key);
+            var existing = has$1.call(obj, key);
             if (existing && options.duplicates === "combine") {
                 obj[key] = utils.combine(obj[key], val);
             } else if (!existing || options.duplicates === "last") {
                 obj[key] = val;
             }
         }
         return obj;
@@ -348547,25 +348681,25 @@
         var key = options.allowDots ? givenKey.replace(/\.([^.[]+)/g, "[$1]") : givenKey;
         var brackets = /(\[[^[\]]*])/;
         var child = /(\[[^[\]]*])/g;
         var segment = options.depth > 0 && brackets.exec(key);
         var parent = segment ? key.slice(0, segment.index) : key;
         var keys2 = [];
         if (parent) {
-            if (!options.plainObjects && has.call(Object.prototype, parent)) {
+            if (!options.plainObjects && has$1.call(Object.prototype, parent)) {
                 if (!options.allowPrototypes) {
                     return;
                 }
             }
             keys2.push(parent);
         }
         var i2 = 0;
         while (options.depth > 0 && (segment = child.exec(key)) !== null && i2 < options.depth) {
             i2 += 1;
-            if (!options.plainObjects && has.call(Object.prototype, segment[1].slice(1, -1))) {
+            if (!options.plainObjects && has$1.call(Object.prototype, segment[1].slice(1, -1))) {
                 if (!options.allowPrototypes) {
                     return;
                 }
             }
             keys2.push(segment[1]);
         }
         if (segment) {
@@ -377025,15 +377159,15 @@
             edge = sourceData.out && sourceData.out[target];
         } else {
             edge = sourceData.undirected && sourceData.undirected[target];
         }
         return edge;
     }
 
-    function isPlainObject$1(value) {
+    function isPlainObject$2(value) {
         return typeof value === "object" && value !== null;
     }
 
     function isEmpty(o2) {
         let k2;
         for (k2 in o2)
             return false;
@@ -377060,15 +377194,15 @@
             descriptor.value = value;
             descriptor.writable = false;
         }
         Object.defineProperty(target, name2, descriptor);
     }
 
     function validateHints(hints) {
-        if (!isPlainObject$1(hints))
+        if (!isPlainObject$2(hints))
             return false;
         if (hints.attributes && !Array.isArray(hints.attributes))
             return false;
         return true;
     }
 
     function incrementalIdStartingFromRandomByte() {
@@ -377396,15 +377530,15 @@
                 this,
                 method,
                 mode,
                 nodeOrEdge,
                 nameOrEdge,
                 add1
             );
-            if (!isPlainObject$1(attributes2))
+            if (!isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     `Graph.${method}: provided attributes are not a plain object.`
                 );
             data2.attributes = attributes2;
             this.emit("nodeAttributesUpdated", {
                 key: data2.key,
                 type: "replace",
@@ -377420,15 +377554,15 @@
                 this,
                 method,
                 mode,
                 nodeOrEdge,
                 nameOrEdge,
                 add1
             );
-            if (!isPlainObject$1(attributes2))
+            if (!isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     `Graph.${method}: provided attributes are not a plain object.`
                 );
             assign$3(data2.attributes, attributes2);
             this.emit("nodeAttributesUpdated", {
                 key: data2.key,
                 type: "merge",
@@ -377773,15 +377907,15 @@
                 element2 = "" + element2;
                 data2 = this._edges.get(element2);
                 if (!data2)
                     throw new NotFoundGraphError(
                         `Graph.${method}: could not find the "${element2}" edge in the graph.`
                     );
             }
-            if (!isPlainObject$1(attributes2))
+            if (!isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     `Graph.${method}: provided attributes are not a plain object.`
                 );
             data2.attributes = attributes2;
             this.emit("edgeAttributesUpdated", {
                 key: data2.key,
                 type: "replace",
@@ -377819,15 +377953,15 @@
                 element2 = "" + element2;
                 data2 = this._edges.get(element2);
                 if (!data2)
                     throw new NotFoundGraphError(
                         `Graph.${method}: could not find the "${element2}" edge in the graph.`
                     );
             }
-            if (!isPlainObject$1(attributes2))
+            if (!isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     `Graph.${method}: provided attributes are not a plain object.`
                 );
             assign$3(data2.attributes, attributes2);
             this.emit("edgeAttributesUpdated", {
                 key: data2.key,
                 type: "merge",
@@ -379068,42 +379202,42 @@
             serialized.attributes = assign$3({}, data2.attributes);
         if (type2 === "mixed" && data2.undirected)
             serialized.undirected = true;
         return serialized;
     }
 
     function validateSerializedNode(value) {
-        if (!isPlainObject$1(value))
+        if (!isPlainObject$2(value))
             throw new InvalidArgumentsGraphError(
                 'Graph.import: invalid serialized node. A serialized node should be a plain object with at least a "key" property.'
             );
         if (!("key" in value))
             throw new InvalidArgumentsGraphError(
                 "Graph.import: serialized node is missing its key."
             );
-        if ("attributes" in value && (!isPlainObject$1(value.attributes) || value.attributes === null))
+        if ("attributes" in value && (!isPlainObject$2(value.attributes) || value.attributes === null))
             throw new InvalidArgumentsGraphError(
                 "Graph.import: invalid attributes. Attributes should be a plain object, null or omitted."
             );
     }
 
     function validateSerializedEdge(value) {
-        if (!isPlainObject$1(value))
+        if (!isPlainObject$2(value))
             throw new InvalidArgumentsGraphError(
                 'Graph.import: invalid serialized edge. A serialized edge should be a plain object with at least a "source" & "target" property.'
             );
         if (!("source" in value))
             throw new InvalidArgumentsGraphError(
                 "Graph.import: serialized edge is missing its source."
             );
         if (!("target" in value))
             throw new InvalidArgumentsGraphError(
                 "Graph.import: serialized edge is missing its target."
             );
-        if ("attributes" in value && (!isPlainObject$1(value.attributes) || value.attributes === null))
+        if ("attributes" in value && (!isPlainObject$2(value.attributes) || value.attributes === null))
             throw new InvalidArgumentsGraphError(
                 "Graph.import: invalid attributes. Attributes should be a plain object, null or omitted."
             );
         if ("undirected" in value && typeof value.undirected !== "boolean")
             throw new InvalidArgumentsGraphError(
                 "Graph.import: invalid undirectedness information. Undirected should be boolean or omitted."
             );
@@ -379139,15 +379273,15 @@
     const DEFAULTS$4 = {
         allowSelfLoops: true,
         multi: false,
         type: "mixed"
     };
 
     function addNode(graph, node2, attributes2) {
-        if (attributes2 && !isPlainObject$1(attributes2))
+        if (attributes2 && !isPlainObject$2(attributes2))
             throw new InvalidArgumentsGraphError(
                 `Graph.addNode: invalid attributes. Expecting an object but got "${attributes2}"`
             );
         node2 = "" + node2;
         attributes2 = attributes2 || {};
         if (graph._nodes.has(node2))
             throw new UsageGraphError(
@@ -379177,15 +379311,15 @@
             throw new UsageGraphError(
                 `Graph.${name2}: you cannot add a directed edge to an undirected graph. Use the #.addEdge or #.addUndirectedEdge instead.`
             );
         if (undirected && graph.type === "directed")
             throw new UsageGraphError(
                 `Graph.${name2}: you cannot add an undirected edge to a directed graph. Use the #.addEdge or #.addDirectedEdge instead.`
             );
-        if (attributes2 && !isPlainObject$1(attributes2))
+        if (attributes2 && !isPlainObject$2(attributes2))
             throw new InvalidArgumentsGraphError(
                 `Graph.${name2}: invalid attributes. Expecting an object but got "${attributes2}"`
             );
         source = "" + source;
         target = "" + target;
         attributes2 = attributes2 || {};
         if (!graph.allowSelfLoops && source === target)
@@ -379272,15 +379406,15 @@
         if (attributes2) {
             if (asUpdater) {
                 if (typeof attributes2 !== "function")
                     throw new InvalidArgumentsGraphError(
                         `Graph.${name2}: invalid updater function. Expecting a function but got "${attributes2}"`
                     );
             } else {
-                if (!isPlainObject$1(attributes2))
+                if (!isPlainObject$2(attributes2))
                     throw new InvalidArgumentsGraphError(
                         `Graph.${name2}: invalid attributes. Expecting an object but got "${attributes2}"`
                     );
             }
         }
         source = "" + source;
         target = "" + target;
@@ -380006,15 +380140,15 @@
             return data2.source === data2.target;
         }
         addNode(node2, attributes2) {
             const nodeData = addNode(this, node2, attributes2);
             return nodeData.key;
         }
         mergeNode(node2, attributes2) {
-            if (attributes2 && !isPlainObject$1(attributes2))
+            if (attributes2 && !isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     `Graph.mergeNode: invalid attributes. Expecting an object but got "${attributes2}"`
                 );
             node2 = "" + node2;
             attributes2 = attributes2 || {};
             let data2 = this._nodes.get(node2);
             if (data2) {
@@ -380215,27 +380349,27 @@
                 type: "remove",
                 attributes: this._attributes,
                 name: name2
             });
             return this;
         }
         replaceAttributes(attributes2) {
-            if (!isPlainObject$1(attributes2))
+            if (!isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     "Graph.replaceAttributes: provided attributes are not a plain object."
                 );
             this._attributes = attributes2;
             this.emit("attributesUpdated", {
                 type: "replace",
                 attributes: this._attributes
             });
             return this;
         }
         mergeAttributes(attributes2) {
-            if (!isPlainObject$1(attributes2))
+            if (!isPlainObject$2(attributes2))
                 throw new InvalidArgumentsGraphError(
                     "Graph.mergeAttributes: provided attributes are not a plain object."
                 );
             assign$3(this._attributes, attributes2);
             this.emit("attributesUpdated", {
                 type: "merge",
                 attributes: this._attributes,
@@ -380495,20 +380629,20 @@
                             this.addUndirectedEdgeWithKey(e3, s2, t2, a2);
                         else
                             this.addDirectedEdgeWithKey(e3, s2, t2, a2);
                     }
                 });
                 return this;
             }
-            if (!isPlainObject$1(data2))
+            if (!isPlainObject$2(data2))
                 throw new InvalidArgumentsGraphError(
                     "Graph.import: invalid argument. Expecting a serialized graph or, alternatively, a Graph instance."
                 );
             if (data2.attributes) {
-                if (!isPlainObject$1(data2.attributes))
+                if (!isPlainObject$2(data2.attributes))
                     throw new InvalidArgumentsGraphError(
                         "Graph.import: invalid attributes. Expecting a plain object."
                     );
                 if (merge2)
                     this.mergeAttributes(data2.attributes);
                 else
                     this.replaceAttributes(data2.attributes);
@@ -389241,18 +389375,18 @@
             _assignValue$1(nested, key, newValue);
             nested = nested[key];
         }
         return object2;
     }
     var _baseSet = baseSet;
 
-    function set(object2, path2, value) {
+    function set$1(object2, path2, value) {
         return object2 == null ? object2 : _baseSet(object2, path2, value);
     }
-    var set_1 = set;
+    var set_1 = set$1;
 
     function copyArray$2(source, array2) {
         var index2 = -1,
             length = source.length;
         array2 || (array2 = Array(length));
         while (++index2 < length) {
             array2[index2] = source[index2];
@@ -409851,15 +409985,15 @@
             for (var j2 = 0; j2 < props.length; j2++) {
                 var prop = props[j2];
                 style2.css(prop.name, prop.value);
             }
         }
         return style2;
     };
-    var version = "3.29.0";
+    var version = "3.29.2";
     var cytoscape$1 = function cytoscape2(options) {
         if (options === void 0) {
             options = {};
         }
         if (plainObject(options)) {
             return new Core(options);
         } else if (string(options)) {
@@ -417603,22 +417737,24 @@
             };
             relativePlacements.push(placement);
         });
         return relativePlacements;
     }
 
     function getTieredLayoutProperties(graph, tiers, orientation, tierSeparation) {
-        const tiersArray = getTiersArray(tiers, graph);
+        let tiersArray = getTiersArray(tiers, graph);
         let nodesOrder;
+        const nodes = graph.nodes();
         if (!Array.isArray(tiers)) {
             const {
                 order_nodes_by
             } = tiers;
-            const nodes = graph.nodes();
             nodesOrder = order_nodes_by ? getNodeOrder(nodes, order_nodes_by, graph) : void 0;
+        } else {
+            tiersArray = tiersArray.map((tier) => tier.filter((node2) => nodes.includes(node2))).filter((filteredTier) => filteredTier.length > 0);
         }
         return {
             alignmentConstraint: tiersArray,
             relativePlacementConstraint: getRelativeTieredArrayPlacement(tiersArray, orientation, tierSeparation, nodesOrder)
         };
     }
     class FcoseLayout extends GraphLayout {
@@ -421198,30 +421334,30 @@
         return isObjectLike$1(value) && getTag$2(value) == mapTag$1;
     }
     var _baseIsMap = baseIsMap$1;
     var baseIsMap = _baseIsMap,
         baseUnary$1 = _baseUnary,
         nodeUtil$1 = _nodeUtil.exports;
     var nodeIsMap = nodeUtil$1 && nodeUtil$1.isMap;
-    var isMap$1 = nodeIsMap ? baseUnary$1(nodeIsMap) : baseIsMap;
-    var isMap_1 = isMap$1;
+    var isMap$2 = nodeIsMap ? baseUnary$1(nodeIsMap) : baseIsMap;
+    var isMap_1 = isMap$2;
     var getTag$1 = _getTag,
         isObjectLike = isObjectLike_1$1;
     var setTag$1 = "[object Set]";
 
     function baseIsSet$1(value) {
         return isObjectLike(value) && getTag$1(value) == setTag$1;
     }
     var _baseIsSet = baseIsSet$1;
     var baseIsSet = _baseIsSet,
         baseUnary = _baseUnary,
         nodeUtil = _nodeUtil.exports;
     var nodeIsSet = nodeUtil && nodeUtil.isSet;
-    var isSet$1 = nodeIsSet ? baseUnary(nodeIsSet) : baseIsSet;
-    var isSet_1 = isSet$1;
+    var isSet$2 = nodeIsSet ? baseUnary(nodeIsSet) : baseIsSet;
+    var isSet_1 = isSet$2;
     var Stack = _Stack,
         arrayEach = _arrayEach,
         assignValue = _assignValue,
         baseAssign = _baseAssign,
         baseAssignIn = _baseAssignIn,
         cloneBuffer = _cloneBuffer.exports,
         copyArray = _copyArray$1,
@@ -421231,17 +421367,17 @@
         getAllKeysIn = _getAllKeysIn,
         getTag = _getTag,
         initCloneArray = _initCloneArray,
         initCloneByTag = _initCloneByTag,
         initCloneObject = _initCloneObject,
         isArray = isArray_1$1,
         isBuffer = isBuffer$4.exports,
-        isMap = isMap_1,
+        isMap$1 = isMap_1,
         isObject$1 = isObject_1$1,
-        isSet = isSet_1,
+        isSet$1 = isSet_1,
         keys = keys_1,
         keysIn = keysIn_1;
     var CLONE_DEEP_FLAG$1 = 1,
         CLONE_FLAT_FLAG = 2,
         CLONE_SYMBOLS_FLAG$1 = 4;
     var argsTag = "[object Arguments]",
         arrayTag = "[object Array]",
@@ -421312,19 +421448,19 @@
         }
         stack || (stack = new Stack());
         var stacked = stack.get(value);
         if (stacked) {
             return stacked;
         }
         stack.set(value, result);
-        if (isSet(value)) {
+        if (isSet$1(value)) {
             value.forEach(function(subValue) {
                 result.add(baseClone$1(subValue, bitmask, customizer, subValue, value, stack));
             });
-        } else if (isMap(value)) {
+        } else if (isMap$1(value)) {
             value.forEach(function(subValue, key2) {
                 result.set(key2, baseClone$1(subValue, bitmask, customizer, key2, value, stack));
             });
         }
         var keysFunc = isFull ? isFlat ? getAllKeysIn : getAllKeys : isFlat ? keysIn : keys;
         var props = isArr ? void 0 : keysFunc(value);
         arrayEach(props || value, function(subValue, key2) {
@@ -425610,14 +425746,672 @@
         }, [allowEdgeAdd, allowNodeDrag, dragMode, editMode]);
         return {
             dragEnabled,
             dragMode,
             setDragMode
         };
     }
+    var __defProp = Object.defineProperty;
+    var __getOwnPropSymbols = Object.getOwnPropertySymbols;
+    var __hasOwnProp = Object.prototype.hasOwnProperty;
+    var __propIsEnum = Object.prototype.propertyIsEnumerable;
+    var __defNormalProp = (obj, key, value) => key in obj ? __defProp(obj, key, {
+        enumerable: true,
+        configurable: true,
+        writable: true,
+        value
+    }) : obj[key] = value;
+    var __spreadValues = (a2, b2) => {
+        for (var prop in b2 || (b2 = {}))
+            if (__hasOwnProp.call(b2, prop))
+                __defNormalProp(a2, prop, b2[prop]);
+        if (__getOwnPropSymbols)
+            for (var prop of __getOwnPropSymbols(b2)) {
+                if (__propIsEnum.call(b2, prop))
+                    __defNormalProp(a2, prop, b2[prop]);
+            }
+        return a2;
+    };
+    var NOTHING = Symbol.for("immer-nothing");
+    var DRAFTABLE = Symbol.for("immer-draftable");
+    var DRAFT_STATE = Symbol.for("immer-state");
+
+    function die(error2, ...args) {
+        throw new Error(
+            `[Immer] minified error nr: ${error2}. Full error at: https://bit.ly/3cXEKWf`
+        );
+    }
+    var getPrototypeOf = Object.getPrototypeOf;
+
+    function isDraft(value) {
+        return !!value && !!value[DRAFT_STATE];
+    }
+
+    function isDraftable(value) {
+        var _a3;
+        if (!value)
+            return false;
+        return isPlainObject$1(value) || Array.isArray(value) || !!value[DRAFTABLE] || !!((_a3 = value.constructor) == null ? void 0 : _a3[DRAFTABLE]) || isMap(value) || isSet(value);
+    }
+    var objectCtorString = Object.prototype.constructor.toString();
+
+    function isPlainObject$1(value) {
+        if (!value || typeof value !== "object")
+            return false;
+        const proto2 = getPrototypeOf(value);
+        if (proto2 === null) {
+            return true;
+        }
+        const Ctor = Object.hasOwnProperty.call(proto2, "constructor") && proto2.constructor;
+        if (Ctor === Object)
+            return true;
+        return typeof Ctor == "function" && Function.toString.call(Ctor) === objectCtorString;
+    }
+
+    function each(obj, iter2) {
+        if (getArchtype(obj) === 0) {
+            Reflect.ownKeys(obj).forEach((key) => {
+                iter2(key, obj[key], obj);
+            });
+        } else {
+            obj.forEach((entry, index2) => iter2(index2, entry, obj));
+        }
+    }
+
+    function getArchtype(thing) {
+        const state = thing[DRAFT_STATE];
+        return state ? state.type_ : Array.isArray(thing) ? 1 : isMap(thing) ? 2 : isSet(thing) ? 3 : 0;
+    }
+
+    function has(thing, prop) {
+        return getArchtype(thing) === 2 ? thing.has(prop) : Object.prototype.hasOwnProperty.call(thing, prop);
+    }
+
+    function set(thing, propOrOldValue, value) {
+        const t2 = getArchtype(thing);
+        if (t2 === 2)
+            thing.set(propOrOldValue, value);
+        else if (t2 === 3) {
+            thing.add(value);
+        } else
+            thing[propOrOldValue] = value;
+    }
+
+    function is(x2, y2) {
+        if (x2 === y2) {
+            return x2 !== 0 || 1 / x2 === 1 / y2;
+        } else {
+            return x2 !== x2 && y2 !== y2;
+        }
+    }
+
+    function isMap(target) {
+        return target instanceof Map;
+    }
+
+    function isSet(target) {
+        return target instanceof Set;
+    }
+
+    function latest(state) {
+        return state.copy_ || state.base_;
+    }
+
+    function shallowCopy(base2, strict) {
+        if (isMap(base2)) {
+            return new Map(base2);
+        }
+        if (isSet(base2)) {
+            return new Set(base2);
+        }
+        if (Array.isArray(base2))
+            return Array.prototype.slice.call(base2);
+        const isPlain = isPlainObject$1(base2);
+        if (strict === true || strict === "class_only" && !isPlain) {
+            const descriptors = Object.getOwnPropertyDescriptors(base2);
+            delete descriptors[DRAFT_STATE];
+            let keys2 = Reflect.ownKeys(descriptors);
+            for (let i2 = 0; i2 < keys2.length; i2++) {
+                const key = keys2[i2];
+                const desc = descriptors[key];
+                if (desc.writable === false) {
+                    desc.writable = true;
+                    desc.configurable = true;
+                }
+                if (desc.get || desc.set)
+                    descriptors[key] = {
+                        configurable: true,
+                        writable: true,
+                        enumerable: desc.enumerable,
+                        value: base2[key]
+                    };
+            }
+            return Object.create(getPrototypeOf(base2), descriptors);
+        } else {
+            const proto2 = getPrototypeOf(base2);
+            if (proto2 !== null && isPlain) {
+                return __spreadValues({}, base2);
+            }
+            const obj = Object.create(proto2);
+            return Object.assign(obj, base2);
+        }
+    }
+
+    function freeze(obj, deep = false) {
+        if (isFrozen(obj) || isDraft(obj) || !isDraftable(obj))
+            return obj;
+        if (getArchtype(obj) > 1) {
+            obj.set = obj.add = obj.clear = obj.delete = dontMutateFrozenCollections;
+        }
+        Object.freeze(obj);
+        if (deep)
+            Object.entries(obj).forEach(([key, value]) => freeze(value, true));
+        return obj;
+    }
+
+    function dontMutateFrozenCollections() {
+        die(2);
+    }
+
+    function isFrozen(obj) {
+        return Object.isFrozen(obj);
+    }
+    var plugins = {};
+
+    function getPlugin(pluginKey) {
+        const plugin = plugins[pluginKey];
+        if (!plugin) {
+            die(0, pluginKey);
+        }
+        return plugin;
+    }
+    var currentScope;
+
+    function getCurrentScope() {
+        return currentScope;
+    }
+
+    function createScope(parent_, immer_) {
+        return {
+            drafts_: [],
+            parent_,
+            immer_,
+            canAutoFreeze_: true,
+            unfinalizedDrafts_: 0
+        };
+    }
+
+    function usePatchesInScope(scope2, patchListener) {
+        if (patchListener) {
+            getPlugin("Patches");
+            scope2.patches_ = [];
+            scope2.inversePatches_ = [];
+            scope2.patchListener_ = patchListener;
+        }
+    }
+
+    function revokeScope(scope2) {
+        leaveScope(scope2);
+        scope2.drafts_.forEach(revokeDraft);
+        scope2.drafts_ = null;
+    }
+
+    function leaveScope(scope2) {
+        if (scope2 === currentScope) {
+            currentScope = scope2.parent_;
+        }
+    }
+
+    function enterScope(immer2) {
+        return currentScope = createScope(currentScope, immer2);
+    }
+
+    function revokeDraft(draft) {
+        const state = draft[DRAFT_STATE];
+        if (state.type_ === 0 || state.type_ === 1)
+            state.revoke_();
+        else
+            state.revoked_ = true;
+    }
+
+    function processResult(result, scope2) {
+        scope2.unfinalizedDrafts_ = scope2.drafts_.length;
+        const baseDraft = scope2.drafts_[0];
+        const isReplaced = result !== void 0 && result !== baseDraft;
+        if (isReplaced) {
+            if (baseDraft[DRAFT_STATE].modified_) {
+                revokeScope(scope2);
+                die(4);
+            }
+            if (isDraftable(result)) {
+                result = finalize(scope2, result);
+                if (!scope2.parent_)
+                    maybeFreeze(scope2, result);
+            }
+            if (scope2.patches_) {
+                getPlugin("Patches").generateReplacementPatches_(
+                    baseDraft[DRAFT_STATE].base_,
+                    result,
+                    scope2.patches_,
+                    scope2.inversePatches_
+                );
+            }
+        } else {
+            result = finalize(scope2, baseDraft, []);
+        }
+        revokeScope(scope2);
+        if (scope2.patches_) {
+            scope2.patchListener_(scope2.patches_, scope2.inversePatches_);
+        }
+        return result !== NOTHING ? result : void 0;
+    }
+
+    function finalize(rootScope, value, path2) {
+        if (isFrozen(value))
+            return value;
+        const state = value[DRAFT_STATE];
+        if (!state) {
+            each(
+                value,
+                (key, childValue) => finalizeProperty(rootScope, state, value, key, childValue, path2)
+            );
+            return value;
+        }
+        if (state.scope_ !== rootScope)
+            return value;
+        if (!state.modified_) {
+            maybeFreeze(rootScope, state.base_, true);
+            return state.base_;
+        }
+        if (!state.finalized_) {
+            state.finalized_ = true;
+            state.scope_.unfinalizedDrafts_--;
+            const result = state.copy_;
+            let resultEach = result;
+            let isSet2 = false;
+            if (state.type_ === 3) {
+                resultEach = new Set(result);
+                result.clear();
+                isSet2 = true;
+            }
+            each(
+                resultEach,
+                (key, childValue) => finalizeProperty(rootScope, state, result, key, childValue, path2, isSet2)
+            );
+            maybeFreeze(rootScope, result, false);
+            if (path2 && rootScope.patches_) {
+                getPlugin("Patches").generatePatches_(
+                    state,
+                    path2,
+                    rootScope.patches_,
+                    rootScope.inversePatches_
+                );
+            }
+        }
+        return state.copy_;
+    }
+
+    function finalizeProperty(rootScope, parentState, targetObject, prop, childValue, rootPath, targetIsSet) {
+        if (isDraft(childValue)) {
+            const path2 = rootPath && parentState && parentState.type_ !== 3 && !has(parentState.assigned_, prop) ? rootPath.concat(prop) : void 0;
+            const res = finalize(rootScope, childValue, path2);
+            set(targetObject, prop, res);
+            if (isDraft(res)) {
+                rootScope.canAutoFreeze_ = false;
+            } else
+                return;
+        } else if (targetIsSet) {
+            targetObject.add(childValue);
+        }
+        if (isDraftable(childValue) && !isFrozen(childValue)) {
+            if (!rootScope.immer_.autoFreeze_ && rootScope.unfinalizedDrafts_ < 1) {
+                return;
+            }
+            finalize(rootScope, childValue);
+            if ((!parentState || !parentState.scope_.parent_) && typeof prop !== "symbol" && Object.prototype.propertyIsEnumerable.call(targetObject, prop))
+                maybeFreeze(rootScope, childValue);
+        }
+    }
+
+    function maybeFreeze(scope2, value, deep = false) {
+        if (!scope2.parent_ && scope2.immer_.autoFreeze_ && scope2.canAutoFreeze_) {
+            freeze(value, deep);
+        }
+    }
+
+    function createProxyProxy(base2, parent) {
+        const isArray2 = Array.isArray(base2);
+        const state = {
+            type_: isArray2 ? 1 : 0,
+            scope_: parent ? parent.scope_ : getCurrentScope(),
+            modified_: false,
+            finalized_: false,
+            assigned_: {},
+            parent_: parent,
+            base_: base2,
+            draft_: null,
+            copy_: null,
+            revoke_: null,
+            isManual_: false
+        };
+        let target = state;
+        let traps = objectTraps;
+        if (isArray2) {
+            target = [state];
+            traps = arrayTraps;
+        }
+        const {
+            revoke,
+            proxy
+        } = Proxy.revocable(target, traps);
+        state.draft_ = proxy;
+        state.revoke_ = revoke;
+        return proxy;
+    }
+    var objectTraps = {
+        get(state, prop) {
+            if (prop === DRAFT_STATE)
+                return state;
+            const source = latest(state);
+            if (!has(source, prop)) {
+                return readPropFromProto(state, source, prop);
+            }
+            const value = source[prop];
+            if (state.finalized_ || !isDraftable(value)) {
+                return value;
+            }
+            if (value === peek(state.base_, prop)) {
+                prepareCopy(state);
+                return state.copy_[prop] = createProxy(value, state);
+            }
+            return value;
+        },
+        has(state, prop) {
+            return prop in latest(state);
+        },
+        ownKeys(state) {
+            return Reflect.ownKeys(latest(state));
+        },
+        set(state, prop, value) {
+            const desc = getDescriptorFromProto(latest(state), prop);
+            if (desc == null ? void 0 : desc.set) {
+                desc.set.call(state.draft_, value);
+                return true;
+            }
+            if (!state.modified_) {
+                const current2 = peek(latest(state), prop);
+                const currentState = current2 == null ? void 0 : current2[DRAFT_STATE];
+                if (currentState && currentState.base_ === value) {
+                    state.copy_[prop] = value;
+                    state.assigned_[prop] = false;
+                    return true;
+                }
+                if (is(value, current2) && (value !== void 0 || has(state.base_, prop)))
+                    return true;
+                prepareCopy(state);
+                markChanged(state);
+            }
+            if (state.copy_[prop] === value && (value !== void 0 || prop in state.copy_) || Number.isNaN(value) && Number.isNaN(state.copy_[prop]))
+                return true;
+            state.copy_[prop] = value;
+            state.assigned_[prop] = true;
+            return true;
+        },
+        deleteProperty(state, prop) {
+            if (peek(state.base_, prop) !== void 0 || prop in state.base_) {
+                state.assigned_[prop] = false;
+                prepareCopy(state);
+                markChanged(state);
+            } else {
+                delete state.assigned_[prop];
+            }
+            if (state.copy_) {
+                delete state.copy_[prop];
+            }
+            return true;
+        },
+        getOwnPropertyDescriptor(state, prop) {
+            const owner = latest(state);
+            const desc = Reflect.getOwnPropertyDescriptor(owner, prop);
+            if (!desc)
+                return desc;
+            return {
+                writable: true,
+                configurable: state.type_ !== 1 || prop !== "length",
+                enumerable: desc.enumerable,
+                value: owner[prop]
+            };
+        },
+        defineProperty() {
+            die(11);
+        },
+        getPrototypeOf(state) {
+            return getPrototypeOf(state.base_);
+        },
+        setPrototypeOf() {
+            die(12);
+        }
+    };
+    var arrayTraps = {};
+    each(objectTraps, (key, fn2) => {
+        arrayTraps[key] = function() {
+            arguments[0] = arguments[0][0];
+            return fn2.apply(this, arguments);
+        };
+    });
+    arrayTraps.deleteProperty = function(state, prop) {
+        return arrayTraps.set.call(this, state, prop, void 0);
+    };
+    arrayTraps.set = function(state, prop, value) {
+        return objectTraps.set.call(this, state[0], prop, value, state[0]);
+    };
+
+    function peek(draft, prop) {
+        const state = draft[DRAFT_STATE];
+        const source = state ? latest(state) : draft;
+        return source[prop];
+    }
+
+    function readPropFromProto(state, source, prop) {
+        var _a3;
+        const desc = getDescriptorFromProto(source, prop);
+        return desc ? `value` in desc ? desc.value : (_a3 = desc.get) == null ? void 0 : _a3.call(state.draft_) : void 0;
+    }
+
+    function getDescriptorFromProto(source, prop) {
+        if (!(prop in source))
+            return void 0;
+        let proto2 = getPrototypeOf(source);
+        while (proto2) {
+            const desc = Object.getOwnPropertyDescriptor(proto2, prop);
+            if (desc)
+                return desc;
+            proto2 = getPrototypeOf(proto2);
+        }
+        return void 0;
+    }
+
+    function markChanged(state) {
+        if (!state.modified_) {
+            state.modified_ = true;
+            if (state.parent_) {
+                markChanged(state.parent_);
+            }
+        }
+    }
+
+    function prepareCopy(state) {
+        if (!state.copy_) {
+            state.copy_ = shallowCopy(
+                state.base_,
+                state.scope_.immer_.useStrictShallowCopy_
+            );
+        }
+    }
+    var Immer2 = class {
+        constructor(config2) {
+            this.autoFreeze_ = true;
+            this.useStrictShallowCopy_ = false;
+            this.produce = (base2, recipe, patchListener) => {
+                if (typeof base2 === "function" && typeof recipe !== "function") {
+                    const defaultBase = recipe;
+                    recipe = base2;
+                    const self2 = this;
+                    return function curriedProduce(base22 = defaultBase, ...args) {
+                        return self2.produce(base22, (draft) => recipe.call(this, draft, ...args));
+                    };
+                }
+                if (typeof recipe !== "function")
+                    die(6);
+                if (patchListener !== void 0 && typeof patchListener !== "function")
+                    die(7);
+                let result;
+                if (isDraftable(base2)) {
+                    const scope2 = enterScope(this);
+                    const proxy = createProxy(base2, void 0);
+                    let hasError = true;
+                    try {
+                        result = recipe(proxy);
+                        hasError = false;
+                    } finally {
+                        if (hasError)
+                            revokeScope(scope2);
+                        else
+                            leaveScope(scope2);
+                    }
+                    usePatchesInScope(scope2, patchListener);
+                    return processResult(result, scope2);
+                } else if (!base2 || typeof base2 !== "object") {
+                    result = recipe(base2);
+                    if (result === void 0)
+                        result = base2;
+                    if (result === NOTHING)
+                        result = void 0;
+                    if (this.autoFreeze_)
+                        freeze(result, true);
+                    if (patchListener) {
+                        const p2 = [];
+                        const ip = [];
+                        getPlugin("Patches").generateReplacementPatches_(base2, result, p2, ip);
+                        patchListener(p2, ip);
+                    }
+                    return result;
+                } else
+                    die(1, base2);
+            };
+            this.produceWithPatches = (base2, recipe) => {
+                if (typeof base2 === "function") {
+                    return (state, ...args) => this.produceWithPatches(state, (draft) => base2(draft, ...args));
+                }
+                let patches, inversePatches;
+                const result = this.produce(base2, recipe, (p2, ip) => {
+                    patches = p2;
+                    inversePatches = ip;
+                });
+                return [result, patches, inversePatches];
+            };
+            if (typeof(config2 == null ? void 0 : config2.autoFreeze) === "boolean")
+                this.setAutoFreeze(config2.autoFreeze);
+            if (typeof(config2 == null ? void 0 : config2.useStrictShallowCopy) === "boolean")
+                this.setUseStrictShallowCopy(config2.useStrictShallowCopy);
+        }
+        createDraft(base2) {
+            if (!isDraftable(base2))
+                die(8);
+            if (isDraft(base2))
+                base2 = current(base2);
+            const scope2 = enterScope(this);
+            const proxy = createProxy(base2, void 0);
+            proxy[DRAFT_STATE].isManual_ = true;
+            leaveScope(scope2);
+            return proxy;
+        }
+        finishDraft(draft, patchListener) {
+            const state = draft && draft[DRAFT_STATE];
+            if (!state || !state.isManual_)
+                die(9);
+            const {
+                scope_: scope2
+            } = state;
+            usePatchesInScope(scope2, patchListener);
+            return processResult(void 0, scope2);
+        }
+        setAutoFreeze(value) {
+            this.autoFreeze_ = value;
+        }
+        setUseStrictShallowCopy(value) {
+            this.useStrictShallowCopy_ = value;
+        }
+        applyPatches(base2, patches) {
+            let i2;
+            for (i2 = patches.length - 1; i2 >= 0; i2--) {
+                const patch2 = patches[i2];
+                if (patch2.path.length === 0 && patch2.op === "replace") {
+                    base2 = patch2.value;
+                    break;
+                }
+            }
+            if (i2 > -1) {
+                patches = patches.slice(i2 + 1);
+            }
+            const applyPatchesImpl = getPlugin("Patches").applyPatches_;
+            if (isDraft(base2)) {
+                return applyPatchesImpl(base2, patches);
+            }
+            return this.produce(
+                base2,
+                (draft) => applyPatchesImpl(draft, patches)
+            );
+        }
+    };
+
+    function createProxy(value, parent) {
+        const draft = isMap(value) ? getPlugin("MapSet").proxyMap_(value, parent) : isSet(value) ? getPlugin("MapSet").proxySet_(value, parent) : createProxyProxy(value, parent);
+        const scope2 = parent ? parent.scope_ : getCurrentScope();
+        scope2.drafts_.push(draft);
+        return draft;
+    }
+
+    function current(value) {
+        if (!isDraft(value))
+            die(10, value);
+        return currentImpl(value);
+    }
+
+    function currentImpl(value) {
+        if (!isDraftable(value) || isFrozen(value))
+            return value;
+        const state = value[DRAFT_STATE];
+        let copy2;
+        if (state) {
+            if (!state.modified_)
+                return state.base_;
+            state.finalized_ = true;
+            copy2 = shallowCopy(value, state.scope_.immer_.useStrictShallowCopy_);
+        } else {
+            copy2 = shallowCopy(value, true);
+        }
+        each(copy2, (key, childValue) => {
+            set(copy2, key, currentImpl(childValue));
+        });
+        if (state) {
+            state.finalized_ = false;
+        }
+        return copy2;
+    }
+    var immer = new Immer2();
+    var produce = immer.produce;
+    immer.produceWithPatches.bind(
+        immer
+    );
+    immer.setAutoFreeze.bind(immer);
+    immer.setUseStrictShallowCopy.bind(immer);
+    immer.applyPatches.bind(immer);
+    immer.createDraft.bind(immer);
+    immer.finishDraft.bind(immer);
 
     function i(f2) {
         var u2 = React.useState(function() {
                 return freeze("function" == typeof f2 ? f2() : f2, true);
             }),
             i2 = u2[1];
         return [u2[0], React.useCallback(function(t2) {
@@ -427954,15 +428748,15 @@
                 invariant(this.isSourceId(sourceId), "Expected a valid source ID.");
                 var isPinned = includePinned && sourceId === this.pinnedSourceId;
                 var source = isPinned ? this.pinnedSource : this.dragSources.get(sourceId);
                 return source;
             }
         }, {
             key: "getTarget",
-            value: function getTarget(targetId) {
+            value: function getTarget2(targetId) {
                 invariant(this.isTargetId(targetId), "Expected a valid target ID.");
                 return this.dropTargets.get(targetId);
             }
         }, {
             key: "getSourceType",
             value: function getSourceType(sourceId) {
                 invariant(this.isSourceId(sourceId), "Expected a valid source ID.");
@@ -431464,15 +432258,15 @@
     overflow-y: auto;
     display: flex;
     flex-direction: column;
     align-items: stretch;
 
     width: 100%;
     height: 100%;
-    padding-top: 12px;
+    padding: 12px 0;
 
     background-color: ${(props) => props.theme.colors.background};
 
     /* Draw a background like in the graph editor */
     background-image: radial-gradient(circle, ${(props) => props.theme.colors.grey2} 1px, transparent 1px);
     background-size: 20px 20px;
 `;
```

## Comparing `dara_components-1.8.5.dist-info/LICENSE` & `dara_components-1.8.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dara_components-1.8.5.dist-info/METADATA` & `dara_components-1.8.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: dara-components
-Version: 1.8.5
+Version: 1.8.6
 Summary: Components for the Dara Framework
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Patricia Jacob
 Author-email: patricia@causalens.com
 Requires-Python: >=3.8.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=3.1.0,<3.2.0)
 Requires-Dist: cai-causal-graph (>=0.3.6)
-Requires-Dist: dara-core (==1.8.5)
+Requires-Dist: dara-core (==1.8.6)
 Requires-Dist: dill (>=0.3.0,<0.4.0)
 Requires-Dist: matplotlib (>=2.0.0)
 Requires-Dist: pandas (>=1.1.0,<3.0.0)
 Requires-Dist: plotly (>=5.14.0,<5.15.0)
 Requires-Dist: scipy
 Requires-Dist: seaborn (>=0.11.0)
 Project-URL: Repository, https://github.com/causalens/dara
 Description-Content-Type: text/markdown
 
 # Dara Components
 
-<img src="https://github.com/causalens/dara/blob/VERSION-1.8.5/img/dara_light.svg?raw=true">
+<img src="https://github.com/causalens/dara/blob/VERSION-1.8.6/img/dara_light.svg?raw=true">
 
 ![Master tests](https://github.com/causalens/dara/actions/workflows/tests.yml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI](https://img.shields.io/pypi/v/dara-components.svg?color=dark-green)](https://pypi.org/project/dara-components/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dara-components.svg?color=dark-green)](https://pypi.org/project/dara-components/)
 [![NPM](https://img.shields.io/npm/v/@darajs/components.svg?color=dark-green)](https://www.npmjs.com/package/@darajs/components)
```

## Comparing `dara_components-1.8.5.dist-info/RECORD` & `dara_components-1.8.6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -74,13 +74,13 @@
 dara/components/smart/data_slicer/data_slicer_modal.py,sha256=t7NywA5DiFiUiUnuFQbTAAVm6PM7Qjd6LGzd9OWA0QE,4120
 dara/components/smart/data_slicer/extension/data_slicer_filter.py,sha256=2wdWn3gcrewrhUZ4tGNwAh1JURpcLmeDKIP7c5j9_sI,1616
 dara/components/smart/data_slicer/extension/filter_status_button.py,sha256=02CgqHEBgkZg1E9v9HGrnRYvEiMNhYpajyOwGuPNV1M,1345
 dara/components/smart/data_slicer/utils/core.py,sha256=6BrmG-iwQCuwUAKQ-y9zFKLeinnzhXIaUOB58UxCYbc,8656
 dara/components/smart/data_slicer/utils/data_preview.py,sha256=OAphjMrm3F76XmJ09X7sZSeOeKqGJFwN5ooo3qcyrG4,1722
 dara/components/smart/data_slicer/utils/plotting.py,sha256=JYzdQLXdAD0A8k2W-764xUr7zN0Ri5nf3OQ2Nb_iuiY,3313
 dara/components/smart/hierarchy.py,sha256=STkgyZiVB1c6KJtcKnn1r8lnjZAIrWkTCpZ_WCyCI1c,2877
-dara/components/umd/dara.components.umd.js,sha256=u6E-We4MQO6wxpPCxsxvy4XdzldjkMfaBYhtfi3chRw,16985599
+dara/components/umd/dara.components.umd.js,sha256=fMV3CmhpXhtfwoHtFCjvi9lUbCH8KknqjsH3HW0nuuc,17002704
 dara/components/umd/style.css,sha256=cvNU48TRRp73QxBrE9awB-zm3YURFnFlASafeLTNa_U,23576
-dara_components-1.8.5.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-dara_components-1.8.5.dist-info/METADATA,sha256=7x0Rwys0oh-a3zLgafXyvuXf2dRvpxocGPl2uZYqTdc,2710
-dara_components-1.8.5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-dara_components-1.8.5.dist-info/RECORD,,
+dara_components-1.8.6.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+dara_components-1.8.6.dist-info/METADATA,sha256=JtPknx-gyz0Uw2-wYKmXlQb44RSYoP8dm-thT6MEgNg,2710
+dara_components-1.8.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+dara_components-1.8.6.dist-info/RECORD,,
```

