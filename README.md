# TVWS Demo Repository

🚀 **Live demo and examples** for the [TVWS](https://github.com/badsector666/tvws) TradingView WebSocket library.

## 🌐 Live Demo

Visit the live demo: **https://badsector666.github.io/tvws-demo/**

## ✨ Features Demonstrated

- **WebSocket Connection** - Connect to TradingView endpoints
- **Authentication Support** - Optional session-based authentication
- **Multiple Symbol Support** - Query multiple trading pairs simultaneously
- **All Timeframes** - Support for every TradingView timeframe (1m to 1M)
- **Performance Metrics** - Connection and data performance monitoring
- **Error Handling** - Comprehensive error management
- **Live Debug Log** - Real-time event monitoring
- **Performance Metrics** - Connection and data performance tracking

## 🚀 Quick Start

### Using the Demo

1. **Visit Live Demo**: [https://badsector666.github.io/tvws-demo/](https://badsector666.github.io/tvws-demo/)
2. **Quick Connect**: Click the "🚀 Quick Connect" button for instant connection
3. **Configure Query**: Enter symbols and select timeframes
4. **Fetch Data**: Click "📊 Get K-Line Data" to retrieve market data

### Local Development

```bash
git clone https://github.com/badsector666/tvws-demo.git
cd tvws-demo
npm install
npm run dev
```

Visit http://localhost:5173 for local development.

### Building for Production

```bash
npm run build
npm run preview
```

## 📊 Supported Symbols

### Forex Pairs
```
FX:EURUSD    # EUR/USD
FX:GBPUSD    # GBP/USD  
FX:USDJPY    # USD/JPY
FX:USDCHF    # USD/CHF
```

### Cryptocurrencies
```
BINANCE:BTCUSDT.P  # Bitcoin/USDT Perpetual
BINANCE:ETHUSDT.P  # Ethereum/USDT Perpetual
CRYPTO:BTCUSD      # Bitcoin/USD
CRYPTO:ETHUSD      # Ethereum/USD
```

### Stocks
```
NASDAQ:AAPL    # Apple Inc.
NASDAQ:GOOGL   # Alphabet Inc.
NYSE:TSLA      # Tesla Inc.
NYSE:BRK.A     # Berkshire Hathaway
```

### Commodities
```
FOREXCOM:XAUUSD  # Gold
FOREXCOM:XAGUSD  # Silver
NYMEX:CL1!       # Crude Oil
```

## ⏰ Available Timeframes

The demo supports all TradingView timeframes:

- **Intraday**: 1m, 3m, 5m, 15m, 30m, 45m, 1h, 2h, 3h, 4h
- **Daily & Above**: 1D, 1W, 1M

## 🛠️ Features

### Quick Connect
- Bypasses all configuration for fastest connection testing
- Uses the most reliable endpoint settings
- Perfect for quick testing and troubleshooting

### Authentication
- Optional TradingView session ID authentication
- Access to premium data endpoints
- Step-by-step authentication guide included

### Performance Monitoring
- Real-time connection performance metrics
- Request timing analysis
- Success rate tracking
- Error reporting and troubleshooting

### Multi-Symbol/Timeframe Support
- Query multiple symbols simultaneously
- Select multiple timeframes at once
- Custom candle amounts per timeframe
- Organized results display

## 🔧 Configuration

### WebSocket Endpoints
- **data** - Standard endpoint (recommended)
- **prodata** - Premium endpoint (requires authentication)
- **widgetdata** - Widget endpoint
- **charts-polygon** - Polygon.io integration

### Authentication
1. Open [TradingView](https://www.tradingview.com/chart/)
2. Open Developer Tools (F12)
3. Go to Application → Cookies → tradingview.com
4. Find and copy the `sessionid` cookie value
5. Enable authentication in the demo and paste the session ID

## 📚 Learn More

### Main Library
- **GitHub**: https://github.com/badsector666/tvws
- **NPM**: https://www.npmjs.com/package/tvws
- **Documentation**: Complete API reference in main repository

### CDN Usage
```html
<script type="module">
import { connect, getCandles } from 'https://unpkg.com/tvws@latest/dist/index.js';

// Use TVWS directly in your browser
const connection = await connect();
const candles = await getCandles({
  connection,
  symbols: ['FX:EURUSD'],
  amount: 100,
  timeframe: '1D'
});
</script>
```

## 🤝 Contributing

We welcome contributions to the demo! Please feel free to:

- Improve the demo interface
- Add new example features  
- Report bugs and issues
- Suggest enhancements
- Submit pull requests

### Development Setup
```bash
# Fork and clone the repository
git clone https://github.com/your-username/tvws-demo.git
cd tvws-demo

# Install dependencies
npm install

# Start development server
npm run dev

# Make your changes...

# Build and test
npm run build
npm run preview
```

## 📄 License

This demo is licensed under the MIT License - same as the main TVWS library.

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/badsector666/tvws-demo/issues)
- **Main Library Support**: [TVWS Repository](https://github.com/badsector666/tvws)
- **Email**: badsectorkiller666@gmail.com

---

**Built with ❤️ for the trading community**

Made with [TVWS](https://github.com/badsector666/tvws) - TradingView WebSocket Library