#include <bits/stdc++.h>
using namespace std;
/* Author------SUNNY KUMAR-------Author */
#define fast()                        \
    ios_base::sync_with_stdio(false); \
    cin.tie(NULL);                    \
    cout.tie(NULL);
#pragma GCC optimize("O3")
#pragma GCC Optimization("unroll-loops")
#pragma GCC target("avx2")
#define ll long long int
#define endl "\n"
#define debug(x)                \
    for (auto element : x)      \
        cout << element << " "; \
    cout << endl;
#define debugp(x)          \
    for (auto element : x) \
        cout << element.first << " " << element.second << endl;
#define db(x) cout << #x << " = " << x << endl;
#define MAX2(x, y) ((x) >= (y) ? (x) : (y))
#define MIN2(x, y) ((x) >= (y) ? (y) : (x))
#define MIN3(x, y, z) MIN2(x, MIN2(y, z))
#define MAX3(x, y, z) MAX2(x, MAX2(y, z))
#define pb push_back
#define pf push_front
#define popf pop_front
#define popb pop_back
const ll MOD = 1e9 + 7;
const ll N = 1e5 + 10;
#define ni1(t) \
    ll t;      \
    cin >> t;
#define ni2(a, b) \
    ll a, b;      \
    cin >> a >> b
#define ni3(a, b, c) \
    ll a, b, c;      \
    cin >> a >> b >> c
#define ni4(a, b, c, d) \
    ll a, b, c, d;      \
    cin >> a >> b >> c >> d
#define ni5(a, b, c, d, e) \
    ll a, b, c, d, e;      \
    cin >> a >> b >> c >> d >> e
#define ni6(a, b, c, d, e, f) \
    ll a, b, c, d, e, f;      \
    cin >> a >> b >> c >> d >> e >> f
#define rep(i, a, b) for (ll i = a; i <= b; i++)
#define revrep(i, a, b) for (ll i = a; i >= b; i--)
#define mem0(a) memset(a, 0, sizeof(a))
#define vll(v, n)    \
    vector<ll> v(n); \
    rep(i, 0, n - 1) { cin >> v[i]; }
#define array(arr, n) \
    ll arr[n];        \
    rep(i, 0, n - 1) cin >> arr[i];
#define arrayx(arr, n, x) \
    ll arr[n];            \
    rep(i, 0, n - 1) arr[i] = x;
#define printarray(arr, n) rep(i, 0, n - 1) cout << arr[i];
/*__________________________________________________________________________________________________________*/
void begin() {
    ll n;
    cin >> n;
    string s;
    cin >> s;
    ll idx = -1;
    bool one = false;
    for (ll i = 0; i < s.size(); i++) {
        if (s[i] == '1') one = true;
        if (s[i] == '0' && one) {
            idx = i;
            break;
        }
    }
    if (idx == -1) {
        cout << 0 << endl;
        return;
    }
    ll length = idx;
    string res = s;
    string rem = "";
    for (ll i = length - 1; i >= 0; i--) {
        rem += s[i];
    }
    for (ll i = 0; i < length; i++) {
        string curr = "";
        string sub = s.substr(i, n - length);
        ll j = s.size() - 1;
        ll k = sub.size() - 1;
        while (k >= 0) {
            if (s[j] == '1' || sub[k] == '1') {
                curr += '1';
            } else {
                curr += '0';
            }
            j--;
            k--;
        }
        curr += rem;

        string rev = string(curr.rbegin(), curr.rend());
        res = max(res, rev);
    }
    bool zero = false;
    for (ll i = 0; i < res.size(); i++) {
        if (res[i] == '0' && zero) {
            cout << res[i];
        }
        if (res[i] == '1') {
            zero = true;
            cout << res[i];
        }
    }
    cout << endl;
}
/*__________________________________________________________________________________________________________*/
int main() {
    /*

    */
    fast();
    ll tc = 1;
    // cin >> tc;
    while (tc--) {
        begin();
    }
    return 0;
}
