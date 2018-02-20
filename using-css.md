The general sibling combinator \(~\) in CSS looks like this in use:

.featured-image ~ p {

font-size: 90%;

}

This selects elements at the same hierarchy level

Select and style every &lt;p&gt; element that are placed immediately after &lt;div&gt; elements:

div + p { 

    background-color: yellow;

}

