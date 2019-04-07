# Tabs

You can use Materialize tabs to show multiple sets of controls on a single page. 

## Creating tabs

You can use `New-UDTabContainer` and `New-UDTab` to create a set of tabs. The `-Text` parameter of `New-UDTab` controls the tabs text while the `-Content` parameter controls the contents of the tab. The contents can be any other UD control. 

```text
New-UDTabContainer -Tabs {
    New-UDTab -Text "Tab 1" -Content {
        New-UDHeading -Text 'This is some text'
    }
    New-UDTab -Text "Tab 2" -Content {
        New-UDHeading -Text 'This is some text'
    }
    New-UDTab -Text "Tab 3" -Content {
        New-UDHeading -Text 'This is some text'
    }
}      
```

This would result in the following tab control. 

![A tab control](../../.gitbook/assets/image%20%281%29.png)

