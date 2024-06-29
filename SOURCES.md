# Sources

Below are all the sources used in this project divided up between each file used in each of the directories for MVVM.

If the source isn't mentioned here it is either our own code or taken from the AlphaVantage API documentation.

Many default files from MAUI are also in the Project.

# General

For MAUI Tutorials and RelayCommand: [James Montemagno](https://www.youtube.com/watch?v=DuNLR_NJv8U)


API Documentation: [Docs](https://www.alphavantage.co/documentation/)

## `Models` Sources

#### `News.cs`

1. Classes are modeled based on [Alpha Vanatge JSON Data](https://www.alphavantage.co/query?function=NEWS_SENTIMENT&tickers=AAPL&apikey=demo)

    (Each property in the JSON is given a class property in `News.cs`)

#### `Stock.cs`

2. Classes are modeled based on [Alpha Vanatge JSON Data](https://www.alphavantage.co/query?function=TIME_SERIES_INTRADAY&symbol=IBM&interval=5min&apikey=demo)

    (Each property in the JSON is given a class property in `Stock.cs`)

## `Services` Sources

#### `AlphaVantageService.cs`

1. Saxion RealWorld Interaction [Networking and async slides](https://learn-eu-central-1-prod-fleet01-xythos.content.blackboardcdn.com/608d78f160587/52090138?X-Blackboard-S3-Bucket=learn-eu-central-1-prod-fleet01-xythos&X-Blackboard-Expiration=1719435600000&X-Blackboard-Signature=J3SYnWtLbAuhTeAIFH%2Bbxm3XFmBC2OcnWS7WPkeIxKY%3D&X-Blackboard-Client-Id=329908&X-Blackboard-S3-Region=eu-central-1&response-cache-control=private%2C%20max-age%3D21600&response-content-disposition=inline%3B%20filename%2A%3DUTF-8%27%27Week%252004%2520Networking.pdf&response-content-type=application%2Fpdf&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEDAaDGV1LWNlbnRyYWwtMSJHMEUCIQDDIOk%2BwA%2BJ9bYvh7m%2FETDEEXE7eF4lONeyMf9RLSTOPAIgKAEv%2FVTIruP%2FF7Hiu0%2BSfcV%2Ban956aQCLPhds92Drx8qxwUI2f%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAEGgw2MzU1Njc5MjQxODMiDOxTDjbVNaE%2F9aNIniqbBfqIwOc%2Bzlbys6EanM%2BCmRS0KVXTf2Nn4e4Z0%2FlRwadf39QkDvPTsyntsdqxCC%2F1qBTWo7QEPT%2FQ9tXc4k59rW5oF9tBAxYGGRWnokRS6%2BHlWuMfES7mxrv58PcjErjcqf9qqwpqfw4dbG7x5nSCJkzls%2BDp%2BvL%2BzB05VNFx2vYga2%2B%2FufdaqkYdrKrdmKjKmsj5LTlleoujglpiHCmbumyvpgKdce12QiYIJO7dJxSPnZ8TRIb7pOG%2B2OXNkQyd%2BScPZ8JwBqLaOCV3KRnbB%2BMjWSnJs3EDhVeN9oydiKIowNSQu2Sd591levGGFrcCFeLjrWH1GMQb%2F4Z7BOGpbEDGnOE2szbb%2FaJKDjAoXN%2F2VzBvEaSWhBZk3zcKsPTRPcnOaEj%2B1sQ3I%2FnDGhWRDB6PVSE1hfuWcGTOdV06TJwgAz5A8R46Tm8JQmcj4LG2WyVUbViYgvQa23JVugMcdkDcanBGth5zLVYmPApOvlFxZ3ApJXU1S1JOX%2FRgE5tysEHfdPHkexduABZSApA9VoL1LTrxsbxvYpr7szCB5CDP92o0vMdyPRyvEpv8rjMCjUVgfraxiHSXo7Wa3NkG2r8eq3jMMAWeYBHGC3zR5c2tQAaVyi1VDeIM1KeDV02eDVUeI8GsgiZYdtBgME%2Bv2VJeQjBNZFoHjHkLkl3X9TmTLza1%2FFfKF27DWBSMRRmAOVDAuw6ytcg7mkSl%2B35XRipvt%2FlJJNgxdoWgdCD9RDSG6pQDgeuSLzt16wgeciML5vWfKG5eLmiV2T8D2aDAMjJYLAn7kHF0uI4ImpXlRJgRapWnY4VVeGdBvxFQqjqM4ojvgzORY5GwQRjsewaC4%2FeEKFOIVMw3X0VIW%2FcZ4RdS2cV3BqMN4cSnQXowkfnwswY6sQEkWhJEpq7gIp6FeBJ9K%2BfrpuhNd63yCzKTWZyIOZiqvCqxN8H1932wUkMvFYYhjFF%2B7AtFSO54audPt7JI%2BY1XbfaXhXbwUVmyseQUp%2Fm8houA3ia8sJO8EKsscn5lEl6oXbSIwpfaGmX4UtnO%2FiuEGVqTkcxyEaLQOys3siwf20BUPl1tnava4SwXS6h3wYhkjtJ%2F6f57Bo%2BjLeqSVWUGzeqgOfwffFNPRZbfGnodEe4%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240626T150000Z&X-Amz-SignedHeaders=host&X-Amz-Expires=21600&X-Amz-Credential=ASIAZH6WM4PL4V534BU4%2F20240626%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=d25a2ff893283b6c726d807233addc4f12002f4d1d4573533305a79c995585dd) on Blackboard.

#### `IAlphaVantageService.cs` 

2. Saxion RealWorld Interaction [Inheritance slides](https://learn-eu-central-1-prod-fleet01-xythos.content.blackboardcdn.com/608d78f160587/51830774?X-Blackboard-S3-Bucket=learn-eu-central-1-prod-fleet01-xythos&X-Blackboard-Expiration=1719435600000&X-Blackboard-Signature=dPHsg9wj3VjXTbcFTDKTpc4SrYMpG%2FhB8oIGVwEc7EI%3D&X-Blackboard-Client-Id=329908&X-Blackboard-S3-Region=eu-central-1&response-cache-control=private%2C%20max-age%3D21600&response-content-disposition=inline%3B%20filename%2A%3DUTF-8%27%27Week%252002%2520Inheritance.pdf&response-content-type=application%2Fpdf&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEDEaDGV1LWNlbnRyYWwtMSJIMEYCIQDWIRSJnI4rk6zfdBfscgYVjrKyBhsVnDxt3o9UApuzhQIhAM%2FMJs2LVpAjaSO3G5mpzk7rPtRpE85pHJFRskQZCK%2F%2FKscFCNr%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQBBoMNjM1NTY3OTI0MTgzIgxDWTA5ZReXJdSLafwqmwUpz4cMfomklYvTzGowRlm9q30CoBJnXAg%2Fs7X8rNXthbTA43%2F2RKthfbJGtj4jbQ3fYBeFo4BhAQqJrci6aN9p3DgoZrI07YJfjgp4zokCMS84LULMWeIs62geWy5UZaD%2BjW6DvBbyVwGnJCv74iHD7bOvYLfn%2F1aEXl%2BgXCTMyPxFVVqMyenWp6XOAzuUGW90lJJeQw388lwk%2BeYEoMbasEFPYiCUG27cFADlFLZUZm6tLFi0hBtDvZ5Ed0fZJFp3SCxhQu%2BZ8XHBENifMiFBq%2B%2BeuB2pd055Nppytk%2BJqNhunUhWWYMC04Gq9vhRG9qSYJqgZOL2ApmTluVyxEu0b9s3f72xE7ig25vvKOoZFCYEJzsOdruAm5lYonO1xyapoHu%2BZlf7T2nESZD2UkAnovpk1Hr1AppGKbNxeDt75zXTFFyghkDqjW2naRg2MESe%2FJn0HrmlX%2BIA%2FkB8hRENWLow481lzVtLkRJNeDlPNZlQlZNZQ%2B8cyT20L8Ya8iIWmvZavKSoZ9NkvPLWfSXR1eG%2BUDJQJXXWCzV8BHDBO4yYOvXCwYEJGcIgl3DxBMskUQK9gnjYWfXuD%2FxE0wlK21my82r50b4uRiOUm2Dp1HiiZXs6uktlVeql6JsYjgixwxJxzrdkSzmKHxUnNbH460JRs5%2FSDzA%2FfOVByJFXJfkRVL8K%2B4yWzz3I1bqdQzMM%2BrY%2F0aaKzSF773eNh05vq4jmmwXt%2BDDCJo2it%2BnMNN1Y6%2FB%2FAjfegafwRV8YxrBN%2FXLxnwq80tOO2qNyY2DtDS2KmqEQUWjGwtkdyttgY%2ByD2svDXzwMzfKbtf4UpiqsjQIDGHIR3GCIH39Mha2ZrCKfYGY%2BbMZpNpCLnoVDXusDPXsUZXmekEyxMPKM8bMGOrABiQBmNulWHNhmvAipbj5IB7xdtK5vWBLCdGA8qrCWmkhhYSwD0Q7Nv6%2BaZBJOiK7fUgVWkwcN1ym7vJRX1RWEECkVPAdzOVe1kjcKeSZpnd9SMKA68p3A285WJyZ9i%2FssIsRHP%2FSTrbDTChCQdogu%2FPhip3YxKJy%2FajGnu0t4651uDz8xkFAIvItQrUlCNvX8y6nqwA%2Blj6aguzmHB1qkLIDR95zPK5%2Bb5L%2BNrMiuoH4%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240626T150000Z&X-Amz-SignedHeaders=host&X-Amz-Expires=21600&X-Amz-Credential=ASIAZH6WM4PLZSR54WW7%2F20240626%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Signature=fc8c4796f3d66fff13f64036e34579b4d40e23cdd7250cb22f858a772857e50a) on Blackboard.

## `Views` Sources

#### `AboutPage.xaml`

1. Default MAUI `dotnet_bot.png` used from resources directory.
2. Button and Binding Properties from [MAUI docs](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/button?view=net-maui-8.0).

#### `MainPage.xaml`

1. Grids from [MAUI Grids Video](https://www.youtube.com/watch?v=hmoe1FMx3Ps).
2. **ChatGPT Usage** - Prompt 

_"How do you bind static text and non-static binding since they cannot be combined in a XAML file"_

Response Code Suggested:

```xml
<Button Grid.Column="0" HorizontalOptions="Center" VerticalOptions="Center" BackgroundColor="Olive">
    <Button.FormattedText>
        <FormattedString>
            <Span Text="Symbol: " />
            <Span Text="{Binding MetaData.Symbol}" />
        </FormattedString>
    </Button.FormattedText>
</Button>
```

3. [Activity Indicator](https://docs.nativescript.org/ui/activity-indicator) code used for checking `IsBusy` property.


#### `NewsDetailsPage.xaml`

1. `Command` attribute of button for commands. [James Montemagno](https://www.youtube.com/watch?v=DuNLR_NJv8U)

#### `NewsPage.xaml`

1. `<Image>` tag for XAML file and [how to bind it with a cdn from the web](https://learn.microsoft.com/en-us/dotnet/maui/user-interface/controls/image?view=net-maui-8.0).
    [Stack Overflow](https://stackoverflow.com/questions/75692776/setting-image-source-in-view-model-in-net-maui-app) answer for further understanding.

2. [GestureRecognizers](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/gestures/tap?view=net-maui-8.0) Recognizes gestures for Navigation between pages of an app.
Again, James Montegamo.

#### `StockDetailPage.xaml`

1. [Basic Candle Sticks - LiveCharts2](https://livecharts.dev/docs/Maui/2.0.0-rc2/samples.financial.basicCandlesticks)

## `ViewModels` Sources

#### `AboutViewModel.cs`
- [Upgrade your app with MVVM concepts](https://learn.microsoft.com/en-us/dotnet/maui/tutorials/notes-mvvm/?view=net-maui-8.0)

#### `BaseViewModel`

Create a BaseViewModel and implement that to 
- NewsDetailsViewModel.cs
- NewsViewModel.cs
- StockDetailViewModel.cs
- StocksViewModel.cs
 
#### `NewsDetailsViewModel.cs`

1. Get News data from NewsViewModel [James Montemagno](https://www.youtube.com/watch?v=DuNLR_NJv8U)

#### `NewsViewModel.cs`

1. `GoToDetailAsync` transfer data from one view to another view. [James Montemagno](https://www.youtube.com/watch?v=DuNLR_NJv8U)

#### `StockDetailViewModel.cs`

1. Get Stock data from StocksViewModel [James Montemagno](https://www.youtube.com/watch?v=DuNLR_NJv8U)

#### `StocksViewModel.cs`

1. `GoToDetailAsync` transfer data from one view to another view. [James Montemagno](https://www.youtube.com/watch?v=DuNLR_NJv8U)