# FiveM-QBCore-Addon-Car-Lua-List-Converter
Ever stumbled onto an old car pack for your FiveM QBCore that has an older style vehicle lua and you need the new style becuase of server updates. 
This quick and easy file allows you to change a big list of old style list into the new style in seconds.

Old format from older server versions
 ['subwrx'] = {
        ['name'] = '2004 Subaru Impreza WRX STI',
        ['brand'] = 'subaru',
        ['model'] = 'subwrx',
        ['price'] = 130000,
        ['category'] = 'subaru',
        ['categoryLabel'] = 'subaru',
        ['hash'] = `subwrx`,
        ['shop'] = 'luxury',
    },

New format used in more up-to-date server versions (empty entry down below)
{ model = '',  name = '',  brand = '', price = 100000, category = 'Add-on: Super', type = 'automobile', shop = 'import' },

This allows for quick and easy conversion of old style into new one to make old car packs/mods work with newwer server versions

List goes into resources/[qb]/qb-core/shared/vehicles.lua

Known 'problem': The conversion adds extra commas that need to be removed for the list to work. Hasn't bothered me enough to look further into it as it is easy to make it work.

Written in Pyton

Free to use and change to fit your needs
