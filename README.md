# MOE-Flutter-Templates

Starter project template for MOE Flutter applications.

## Installation

Add as a starting point (or copy the skeleton) into your app:

```yaml
dependencies:
  moe_flutter_templates:
    git:
      url: https://github.com/mindofemanizer/MOE-Flutter-Templates.git
      ref: master
```

## Usage

Bundles the core MOE packages so a new app boots with commerce, payment, and inventory out of the box:

```dart
import 'package:moe_flutter_templates/moe_flutter_templates.dart';
import 'package:moe_flutter_foundation/moe_flutter_foundation.dart';

void main() async {
  WidgetsFlutterBinding.ensureInitialized();

  await MoeFoundation.setup(
    envConfig: EnvConfig.fromEnvironment(),
    environment: Environment.production,
  );

  runApp(MoeFoundationProviderScope(child: const MyApp()));
}
```

## What's Included

| Package | Description |
|---------|-------------|
| `moe_flutter_foundation` | Bundles Core + Settings + Profiles + Auth |
| `moe_flutter_commerce` | Store, product, cart, order |
| `moe_flutter_payment` | Payment gateway integration |
| `moe_flutter_inventory` | Inventory items, warehouses, stock movements |

## Next Steps

1. Copy this package as the base of your new app.
2. Configure `EnvConfig` via `--dart-define` (app name, API base URL, primary color).
3. Extend with any additional MOE packages (`chat`, `crm`, `marketing`, etc.).
